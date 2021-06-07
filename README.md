## 文字轮播

### 使用介绍

#### 安装

```js
npm install world-slide

//or

yarn add world-slide

```

#### 使用
```js
import WorldCarousel from 'world-slide'

const  dataList = [
  {
    label: '东临碣石，以观沧海。',
    date: '2021-05-06'
  },
  {
    label: '水何澹澹，山岛竦峙。',
    date: '2021-05-06'
  },
  {
    label: '树木丛生，百草丰茂。',
    date: '2021-05-06'
  },
  {
    label: '秋风萧瑟，洪波涌起。',
    date: '2021-05-06'
  }
]

const createItemNode = (itemData) => {
  //  内容渲染函数，可不传
  return span>{`${itemData.label}---${itemData.date}`}</span>
}

/*
 * dataList 数据源
 * liHeight 每一条数据的高度
 * speed 速度，单位秒（s）
 * createItemNode 内容渲染函数
 * */

<WorldCarousel dataList={dataList} liHeight={60} speed={3} createItemNode={createItemNode}/>
```