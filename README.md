# Csharpier (Formatter)

    > Learning C# as my T-shaped learning.

Primary purpose of making two repos is that i wanted to check how C# works with and without template.
Conclusion: Not much difference, you can run C# project even without template.

## I wanted something that AI Vibe coders cant do easily and I found it, its C#.
## Learnings Today
- I looked this Csharpier formatter, It formats C# code because traditional Prettier doesn't format C# code.
- But it doesn't work as simply as Prettier ("Prettier" just works out of the box directly when you install the extension and change the default formatter in "User Settings").
- You still do the default formatter stuff (Csharpier extension is just the bridge to the actual tool).

### Csharpier Setup
- For Csharpier to work: 
- You install the Csharpier extension in VS code: The extension only works as a bridge to the orignal tool.
- Install the Csharpier extension globally with the help of dotnet : `dotnet tool install -g csharpier`

### A Thing about Csharpier
- It only formats when the code is syntactically correct. Becuase it build AST (Abstract Syntax Tree), which I learnt in Compiler Construction.

### .sln (solution file)
I haven't seen a direct alternate of .sln file in js, but you can keep in mind that:
A .sln(solution file) can file can keep projects connected/linked, for intellisense purposes and autocompletions etc.

### dotnet CLI
- Talking about dotnet CLI, it acts as both package manager and a runtime environment and two more things that would are more clear to me in JS referance, here is a comparison table in contrast to JavaScript:

| Responsibility | .NET Ecosystem | Node.js Ecosystem |
| --- | --- | --- |
| **Runtime Engine** | .NET CLR | Node.js (V8 Engine) |
| **Package Manager** | `dotnet` (interfacing with NuGet) | `npm` (or `yarn` / `pnpm`) |
| **CLI Tool Runner** | `dotnet tool run` / `csharpier` | `npx` |
| **Compiler / Build** | `dotnet build` / Roslyn | Babel / TypeScript (`tsc`) / Esbuild |