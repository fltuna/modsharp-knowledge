# Sharp.Modules.ClientPreferences.Shared

Project: Sharp.Modules.ClientPreferences.Shared
Types: 4 (0 generated)

### enum CookieValueType : System.Enum

- FullName: `Sharp.Modules.ClientPreferences.Shared.CookieValueType`
- Kind: enum
- Modifiers: public
- Source: Sharp.Modules/ClientPreferences/Shared/CookieValueType.cs:22
- Generated: false

Inheritance: object → System.ValueType → System.Enum → **CookieValueType**

#### Enum Members
- `Sharp.Modules.ClientPreferences.Shared.CookieValueType.Double = 1` [L:32]
  - Modifiers: public, static, const
  - Summary: 浮点数
- `Sharp.Modules.ClientPreferences.Shared.CookieValueType.Number = 0` [L:27]
  - Modifiers: public, static, const
  - Summary: 整数
- `Sharp.Modules.ClientPreferences.Shared.CookieValueType.String = 2` [L:37]
  - Modifiers: public, static, const
  - Summary: 字符串


### interface IClientPreference

- FullName: `Sharp.Modules.ClientPreferences.Shared.IClientPreference`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/ClientPreferences/Shared/IClientPreference.cs:26
- Generated: false

#### Fields
- `const string Sharp.Modules.ClientPreferences.Shared.IClientPreference.Identity = "IClientPreference"` [L:28]
  - Modifiers: public, static, const

#### Methods
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem Sharp.Modules.ClientPreferences.Shared.IClientPreference.SetCookie(Sharp.Shared.Units.SteamID identity, string key, bool value)` [L:53]
  - Modifiers: public, abstract
  - Summary: 设置Cookie
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem Sharp.Modules.ClientPreferences.Shared.IClientPreference.SetCookie(Sharp.Shared.Units.SteamID identity, string key, double value)` [L:63]
  - Modifiers: public, abstract
  - Summary: 设置Cookie
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem Sharp.Modules.ClientPreferences.Shared.IClientPreference.SetCookie(Sharp.Shared.Units.SteamID identity, string key, long value)` [L:58]
  - Modifiers: public, abstract
  - Summary: 设置Cookie
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem Sharp.Modules.ClientPreferences.Shared.IClientPreference.SetCookie(Sharp.Shared.Units.SteamID identity, string key, string value)` [L:68]
  - Modifiers: public, abstract
  - Summary: 设置Cookie
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem Sharp.Modules.ClientPreferences.Shared.IClientPreference.SetCookie<T>(Sharp.Shared.Units.SteamID identity, string key, T value) where T : Sharp.Modules.ClientPreferences.Shared.ISerializableCookieItem<T>` [L:73]
  - Modifiers: public, abstract
  - Summary: 设置 Cookie
- `Sharp.Modules.ClientPreferences.Shared.ICookieItem? Sharp.Modules.ClientPreferences.Shared.IClientPreference.GetCookie(Sharp.Shared.Units.SteamID identity, string key)` [L:43]
  - Modifiers: public, abstract
  - Summary: 获取Cookie
- `System.IDisposable Sharp.Modules.ClientPreferences.Shared.IClientPreference.ListenOnLoad(System.Action<Sharp.Shared.Objects.IGameClient> callback)` [L:33]
  - Modifiers: public, abstract
  - Summary: 监听加载事件, 需要你在Unload或取消监听时进行Dispose
- `bool Sharp.Modules.ClientPreferences.Shared.IClientPreference.DeleteCookie(Sharp.Shared.Units.SteamID identity, string key)` [L:48]
  - Modifiers: public, abstract
  - Summary: 删除Cookie
- `bool Sharp.Modules.ClientPreferences.Shared.IClientPreference.IsLoaded(Sharp.Shared.Units.SteamID identity)` [L:38]
  - Modifiers: public, abstract
  - Summary: 检查是否已经加载数据


### interface ICookieItem

- FullName: `Sharp.Modules.ClientPreferences.Shared.ICookieItem`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/ClientPreferences/Shared/ICookieItem.cs:24
- Generated: false

#### Properties
- `Sharp.Modules.ClientPreferences.Shared.CookieValueType Sharp.Modules.ClientPreferences.Shared.ICookieItem.Type` [L:29]
  - Modifiers: public, abstract, readonly
  - Summary: 类型

#### Methods
- `T Sharp.Modules.ClientPreferences.Shared.ICookieItem.Get<T>() where T : System.Enum` [L:54]
  - Modifiers: public, abstract
  - Summary: 取整数并转换类型为你定义的枚举
- `T Sharp.Modules.ClientPreferences.Shared.ICookieItem.GetObject<T>() where T : Sharp.Modules.ClientPreferences.Shared.ISerializableCookieItem<T>` [L:61]
  - Modifiers: public, abstract
  - Summary: 取字符串并反序列化为你定义的类型
- `double Sharp.Modules.ClientPreferences.Shared.ICookieItem.GetDouble()` [L:41]
  - Modifiers: public, abstract
  - Summary: 取浮点数
- `long Sharp.Modules.ClientPreferences.Shared.ICookieItem.GetNumber()` [L:35]
  - Modifiers: public, abstract
  - Summary: 取整数
- `string Sharp.Modules.ClientPreferences.Shared.ICookieItem.GetString()` [L:47]
  - Modifiers: public, abstract
  - Summary: 取字符串


### interface ISerializableCookieItem<T> : Sharp.Modules.ClientPreferences.Shared.ICookieItem

- FullName: `Sharp.Modules.ClientPreferences.Shared.ISerializableCookieItem<T>`
- Kind: interface
- Modifiers: public
- Source: Sharp.Modules/ClientPreferences/Shared/ISerializableCookieItem.cs:22
- Generated: false
- Constraint: `where T : notnull`

#### Methods
- `T Sharp.Modules.ClientPreferences.Shared.ISerializableCookieItem<out T>.Deserialize(string body)` [L:32]
  - Modifiers: public, static, abstract
  - Summary: 反序列化实现
- `string Sharp.Modules.ClientPreferences.Shared.ISerializableCookieItem<out T>.Serialize()` [L:27]
  - Modifiers: public, abstract
  - Summary: 序列化实现


