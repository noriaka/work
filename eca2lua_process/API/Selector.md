# Selector

选取器

用来选取某个区域内的单位

## count

```lua
(method) Selector:count(count: integer)
  -> Selector
```

 选项 - 选取的数量
## create

```lua
function Selector.create()
  -> Selector
```

 创建选取器
## get

```lua
(method) Selector:get()
  -> UnitGroup
```

 进行选取
## in_shape

```lua
(method) Selector:in_shape(pos: Point, shape: Shape)
  -> Selector
```

 形状 - 添加形状对象
## in_state

```lua
(method) Selector:in_state(state: integer)
  -> Selector
```

 条件 - 拥有某个特定的状态
## include_dead

```lua
(method) Selector:include_dead()
  -> Selector
```

 选项 - 包含死亡的单位
## is_unit_key

```lua
(method) Selector:is_unit_key(unit_key: py.UnitKey)
  -> Selector
```

 条件 - 是某个特定的单位类型
## is_unit_type

```lua
(method) Selector:is_unit_type(unit_type: py.UnitType)
  -> Selector
```

 条件 - 是某个特定的单位类型
## is_visible

```lua
(method) Selector:is_visible(p: Player)
  -> Selector
```

 条件 - 对某个玩家可见
## not_in_group

```lua
(method) Selector:not_in_group(ug: UnitGroup)
  -> Selector
```

 条件 - 不在某个单位组中
## not_in_state

```lua
(method) Selector:not_in_state(state: integer)
  -> Selector
```

 条件 - 不拥有某个特定的状态
## not_is

```lua
(method) Selector:not_is(u: Unit)
  -> Selector
```

 条件 - 不是某个特定的单位
## not_visible

```lua
(method) Selector:not_visible(p: Player)
  -> Selector
```

 条件 - 对某个玩家不可见
## of_player

```lua
(method) Selector:of_player(p: Player)
  -> Selector
```

 条件 - 属于某个玩家
## with_tag

```lua
(method) Selector:with_tag(tag: string)
  -> Selector
```

 条件 - 拥有特定标签
## without_tag

```lua
(method) Selector:without_tag(tag: string)
  -> Selector
```

 条件 - 不拥有特定标签

