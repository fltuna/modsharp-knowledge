# Sharp.Modules.LocalizerManager.Shared

Project: Sharp.Modules.LocalizerManager.Shared
Types: 5 (0 generated)

### interface ILocale

- FullName: `Sharp.Modules.LocalizerManager.Shared.ILocale`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/LocalizerManager/Shared/ILocale.cs:28
- Generated: false
- Summary: Client/culture-scoped locale view (new ergonomic API).

#### Properties
- `System.Globalization.CultureInfo Sharp.Modules.LocalizerManager.Shared.ILocale.Culture` [L:33]
  - Modifiers: public, abstract, readonly
  - Summary: Effective culture for this locale.

#### Methods
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage Sharp.Modules.LocalizerManager.Shared.ILocale.Literal(string text)` [L:93]
  - Modifiers: public, abstract
  - Summary: Convenience for Message().Literal(text).
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage Sharp.Modules.LocalizerManager.Shared.ILocale.Localized(string key, params System.ReadOnlySpan<object?> args)` [L:88]
  - Modifiers: public, abstract
  - Summary: Convenience for Message().Text(key, args).
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage Sharp.Modules.LocalizerManager.Shared.ILocale.Message()` [L:83]
  - Modifiers: public, abstract
  - Summary: Create a fluent message builder bound to this locale/client.
- `bool Sharp.Modules.LocalizerManager.Shared.ILocale.TryText(string key, out string value, object? arg0)` [L:68]
  - Modifiers: public, abstract
  - Summary: Try to localize a key; returns false and key if missing or format fails.
- `bool Sharp.Modules.LocalizerManager.Shared.ILocale.TryText(string key, out string value, object? arg0, object? arg1)` [L:73]
  - Modifiers: public, abstract
  - Summary: Try to localize a key; returns false and key if missing or format fails.
- `bool Sharp.Modules.LocalizerManager.Shared.ILocale.TryText(string key, out string value, object? arg0, object? arg1, object? arg2)` [L:78]
  - Modifiers: public, abstract
  - Summary: Try to localize a key; returns false and key if missing or format fails.
- `bool Sharp.Modules.LocalizerManager.Shared.ILocale.TryText(string key, out string value, params System.ReadOnlySpan<object?> args)` [L:63]
  - Modifiers: public, abstract
  - Summary: Try to localize a key; returns false and key if missing or format fails.
- `string Sharp.Modules.LocalizerManager.Shared.ILocale.Raw(string key, params System.ReadOnlySpan<object?> args)` [L:58]
  - Modifiers: public, abstract
  - Summary: Localize a key ignoring culture (raw string.Format).
- `string Sharp.Modules.LocalizerManager.Shared.ILocale.Text(string key, object? arg0)` [L:43]
  - Modifiers: public, abstract
  - Summary: Localize a key using the locale's culture.
- `string Sharp.Modules.LocalizerManager.Shared.ILocale.Text(string key, object? arg0, object? arg1)` [L:48]
  - Modifiers: public, abstract
  - Summary: Localize a key using the locale's culture.
- `string Sharp.Modules.LocalizerManager.Shared.ILocale.Text(string key, object? arg0, object? arg1, object? arg2)` [L:53]
  - Modifiers: public, abstract
  - Summary: Localize a key using the locale's culture.
- `string Sharp.Modules.LocalizerManager.Shared.ILocale.Text(string key, params System.ReadOnlySpan<object?> args)` [L:38]
  - Modifiers: public, abstract
  - Summary: Localize a key using the locale's culture.


### interface ILocalizedMessage

- FullName: `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/LocalizerManager/Shared/ILocalizedMessage.cs:28
- Generated: false
- Summary: Fluent localized message builder (new ergonomic API).

#### Methods
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage.Literal(string text)` [L:39]
  - Modifiers: public, abstract
  - Summary: Append literal text.
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage.Prefix(string? prefix)` [L:34]
  - Modifiers: public, abstract
  - Summary: Sets the prefix.
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage.Text(string key, params System.ReadOnlySpan<object?> args)` [L:44]
  - Modifiers: public, abstract
  - Summary: Append localized text.
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage.TextOrFallback(string key, string fallback, params System.ReadOnlySpan<object?> args)` [L:49]
  - Modifiers: public, abstract
  - Summary: Append localized text or fallback if missing/format fails.
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage.Transform(System.Func<string, string> processor)` [L:60]
  - Modifiers: public, abstract
  - Summary: Register a post-processor for the rendered string (applied before Build/Print return/send).
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage.Value(object? value)` [L:54]
  - Modifiers: public, abstract
  - Summary: Append a raw value.
- `string Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage.Build()` [L:65]
  - Modifiers: public, abstract
  - Summary: Build the final string (applies prefix/colors and any processors).
- `void Sharp.Modules.LocalizerManager.Shared.ILocalizedMessage.Print([Sharp.Shared.Enums.HudPrintChannel channel = Sharp.Shared.Enums.HudPrintChannel.Chat])` [L:71]
  - Modifiers: public, abstract
  - Summary: Print to the bound client (if any) on the specified channel.


### interface ILocalizedMessageMany

- FullName: `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/LocalizerManager/Shared/ILocalizedMessageMany.cs:28
- Generated: false
- Summary: Fluent localized message builder bound to a captured client set.

#### Methods
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany.Literal(string text)` [L:39]
  - Modifiers: public, abstract
  - Summary: Append literal text.
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany.Prefix(string? prefix)` [L:34]
  - Modifiers: public, abstract
  - Summary: Sets the prefix.
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany.Text(string key, params System.ReadOnlySpan<object?> args)` [L:44]
  - Modifiers: public, abstract
  - Summary: Append localized text.
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany.TextOrFallback(string key, string fallback, params System.ReadOnlySpan<object?> args)` [L:49]
  - Modifiers: public, abstract
  - Summary: Append localized text or fallback if missing/format fails.
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany.Transform(System.Func<string, string> processor)` [L:59]
  - Modifiers: public, abstract
  - Summary: Register a post-processor for each rendered string (applied before print). Multiple calls compose in order.
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany.Value(object? value)` [L:54]
  - Modifiers: public, abstract
  - Summary: Append a raw value.
- `void Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany.Print([Sharp.Shared.Enums.HudPrintChannel channel = Sharp.Shared.Enums.HudPrintChannel.Chat])` [L:64]
  - Modifiers: public, abstract
  - Summary: Render per locale and print to the captured clients. Do not cache builders across reload/unload.


### interface ILocalizerManager

- FullName: `Sharp.Modules.LocalizerManager.Shared.ILocalizerManager`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/LocalizerManager/Shared/ILocalizerManager.cs:27
- Generated: false

#### Fields
- `const string Sharp.Modules.LocalizerManager.Shared.ILocalizerManager.Identity = "ILocalizerManager"` [L:29]
  - Modifiers: public, static, const

#### Methods
- `Sharp.Modules.LocalizerManager.Shared.ILocale Sharp.Modules.LocalizerManager.Shared.ILocalizerManager.For(Sharp.Shared.Objects.IGameClient client)` [L:59]
  - Modifiers: public, abstract
  - Summary: Get a locale bound to a specific client (preferred entrypoint).
- `Sharp.Modules.LocalizerManager.Shared.IMultiLocale Sharp.Modules.LocalizerManager.Shared.ILocalizerManager.ForMany(System.Collections.Generic.IEnumerable<Sharp.Shared.Objects.IGameClient> clients)` [L:64]
  - Modifiers: public, abstract
  - Summary: Get a multi-locale builder for a set of clients (renders per locale).
- `Sharp.Modules.LocalizerManager.Shared.IMultiLocale Sharp.Modules.LocalizerManager.Shared.ILocalizerManager.ForMany(params Sharp.Shared.Objects.IGameClient[] clients)` [L:69]
  - Modifiers: public, abstract
  - Summary: Get a multi-locale builder for a set of clients (renders per locale).
- `string Sharp.Modules.LocalizerManager.Shared.ILocalizerManager.Format(System.Globalization.CultureInfo culture, string key, params System.ReadOnlySpan<object?> args)` [L:45]
  - Modifiers: public, abstract
  - Summary: Format a localized message for server-side usage (logging, webhooks).
- `string Sharp.Modules.LocalizerManager.Shared.ILocalizerManager.Format(string cultureName, string key, params System.ReadOnlySpan<object?> args)` [L:54]
  - Modifiers: public, abstract
  - Summary: Format a localized message for server-side usage (logging, webhooks).
- `void Sharp.Modules.LocalizerManager.Shared.ILocalizerManager.LoadLocaleFile(string name, [bool suppressDuplicationWarnings = false])` [L:36]
  - Modifiers: public, abstract
  - Summary: Load a locale file from {sharp}/locales/{name}.json.


### interface IMultiLocale

- FullName: `Sharp.Modules.LocalizerManager.Shared.IMultiLocale`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/LocalizerManager/Shared/IMultiLocale.cs:27
- Generated: false
- Summary: Locale view for a captured set of clients; intended only for multi-send builders.

#### Methods
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany Sharp.Modules.LocalizerManager.Shared.IMultiLocale.Literal(string text)` [L:42]
  - Modifiers: public, abstract
  - Summary: Convenience for Message().Literal(text).
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany Sharp.Modules.LocalizerManager.Shared.IMultiLocale.Localized(string key, params System.ReadOnlySpan<object?> args)` [L:37]
  - Modifiers: public, abstract
  - Summary: Convenience for Message().Text(key, args).
- `Sharp.Modules.LocalizerManager.Shared.ILocalizedMessageMany Sharp.Modules.LocalizerManager.Shared.IMultiLocale.Message()` [L:32]
  - Modifiers: public, abstract
  - Summary: Create a fluent message builder for the captured clients.


