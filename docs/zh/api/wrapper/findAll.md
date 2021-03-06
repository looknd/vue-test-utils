## findAll(selector)

返回一个 [`WrapperArray`](../wrapper-array/)。

可以使用任何有效的[选择器](../selectors.md)。

- **参数：**
  - `{string|Component} selector`

- **返回值：**`{WrapperArray}`

- **示例：**

```js
import { mount } from '@vue/test-utils'
import Foo from './Foo.vue'
import Bar from './Bar.vue'

const wrapper = mount(Foo)
const div = wrapper.findAll('div').at(0)
expect(div.is('div')).toBe(true)
const bar = wrapper.findAll(Bar).at(0)
expect(bar.is(Bar)).toBe(true)
```
