# Reload

热重载

热重载相关的方法，详细请看 `演示/热重载`。

## afterReloadCallbacks

```lua
{ name: string, callback: Reload.afterReloadCallback }[]
```

## beforeReloadCallbacks

```lua
{ name: string, callback: Reload.beforeReloadCallback }[]
```

## defaultReloadOptional

```lua
nil
```

## filter

```lua
(fun(name: string, reload: Reload):boolean)?
```

## fire

```lua
(method) Reload:fire()
```

## getCurrentIncludeName

```lua
function Reload.getCurrentIncludeName()
  -> string?
```

## include

```lua
function Reload.include(name: string)
  -> any
```

 类似于 `require` ，但是会在重载时重新加载文件。
## includeStack

```lua
table
```

## includedNameMap

```lua
{ [string]: boolean }
```

## includedNames

```lua
string[]
```

## isValidName

```lua
(method) Reload:isValidName(name?: string)
  -> boolean
```

 模块名是否会被重载
## onAfterReload

```lua
function Reload.onAfterReload(callback: Reload.afterReloadCallback)
```

 注册在重载之后的回调
## onBeforeReload

```lua
function Reload.onBeforeReload(callback: Reload.beforeReloadCallback)
```

 注册在重载之前的回调
## optional

```lua
(Reload.Optional)?
```

## reload

```lua
function Reload.reload(optional?: Reload.Optional)
```

 进行重载
## setDefaultOptional

```lua
function Reload.setDefaultOptional(optional?: Reload.Optional)
```

 设置默认的重载选项
## validMap

```lua
table<string, any>
```


# Reload.Optional

## filter

```lua
fun(name: string, reload: Reload):boolean
```

过滤函数
## list

```lua
string[]
```

要重载的模块列表

# Reload.afterReloadCallback


```lua
fun(reload: Reload, hasReloaded: boolean)
```


# Reload.beforeReloadCallback


```lua
fun(reload: Reload, willReload: boolean)
```


