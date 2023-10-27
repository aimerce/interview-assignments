# TypeScript Frontend Engineer Assignment

## 要求

- 参考设计稿实现轮播图的效果
- 封装为 `<Carousel>` 组件
- 数据来源于服务端

Figma设计稿参考地址：
https://www.figma.com/file/JP9zSbA8F8hqPKoAuZ1zxB/Banner?type=design&node-id=0-1&mode=design&t=X7xr8Rea7vTl7oGP-0

轮播图的参考数据结构

```typescript
interface SliderImage {
  id: string;
  link: string;
}

interface SliderItem {
  id: string;
  title: string;
  description: string;
  buttonText: string;
  component: string;
  backgroundImage: SliderImage;
}

interface Slider {
  id: string;
  data: SliderItem[];
}
```

服务端API包含增删改查：

```
GET     /carousel/list
POST    /carousel/add
DELETE  /carousel/delete/:id
PUT     /carousel/update/:id
```

## 加分项

* 良好的代码程序分层结构
* 代码保持简洁/有效/易读
* 还原设计稿，并有更好的交互性
* 响应式设计
* 缓存

## 推荐技术栈

* TypeScript
* React and hooks
* axios
* tailwindcss