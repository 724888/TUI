::: demo
> 使用 `multiple` 开启多选传入value为 `Array` 类型，使用 `collapse-tags` 可收起选项只展示数字
```html
<t-select label="请选择" v-model="v" multiple>
  <t-option v-for="o in options" :key="o.val" :label="o.label" :val="o.val"/>
</t-select>

<t-select label="请选择" v-model="v" multiple collapse-tags>
  <t-option v-for="o in options" :key="o.val" :label="o.label" :val="o.val"/>
</t-select>

<script>
export default {
  data () {
    return {
      v: ['2'],
      options: [
        {label: '北京烤鸭', val: '1'},
        {label: '冷吃牛肉', val: '2'},
        {label: '驴肉火烧', val: '3'},
        {label: '宫保鸡丁', val: '4'},
        {label: '黄焖鸡米饭', val: '5'}
      ]
    }
  }
}
</script>
```
:::
