# Sharp.Shared.Abstractions

Project: Sharp.Shared
Types: 2 (0 generated)

### interface ISharpExtension

- FullName: `Sharp.Shared.Abstractions.ISharpExtension`
- Kind: interface
- Modifiers: public
- Source: Sharp.Shared/Abstractions/ISharpExtension.cs:29
- Generated: false
- Summary: This interface use only for Extensions package. if you want to inherit this, you need to know what you are doing.

#### Methods
- `void Sharp.Shared.Abstractions.ISharpExtension.Load()` [L:31]
  - Modifiers: public, abstract
- `void Sharp.Shared.Abstractions.ISharpExtension.Shutdown()` [L:33]
  - Modifiers: public, abstract


### class SharpExtensionExtensions

- FullName: `Sharp.Shared.Abstractions.SharpExtensionExtensions`
- Kind: class
- Modifiers: public, static
- Source: Sharp.Shared/Abstractions/ISharpExtension.cs:36
- Generated: false

Inheritance: object → **SharpExtensionExtensions**

#### Methods
- `static void Sharp.Shared.Abstractions.SharpExtensionExtensions.LoadAllSharpExtensions(System.IServiceProvider services)` [L:41]
  - Modifiers: public, static, this
  - Summary: Call Load method of all registered ISharpExtension services.
- `static void Sharp.Shared.Abstractions.SharpExtensionExtensions.ShutdownAllSharpExtensions(System.IServiceProvider services)` [L:52]
  - Modifiers: public, static, this
  - Summary: Call Shutdown method of all registered ISharpExtension services.


