# TypeScript Backend Engineer Assignment

### Typescript 实现轮播图数据的后端服务（细节可以百度/谷歌）

撰写 API 接口

- 轮播图相关接口：

  - 创建：接受前端来的轮播图结构，返回创建成功的轮播图实体信息
  - 修改：接受前端发来的轮播图修改信息，返回修改后的轮播图实体信息
  - 读取：通过轮播图 id 查询轮播图数据，返回查询的结果

- 图片上传接口
  - 前端会通过 html form 形式发送一个图片文件和 slider id 过来，请保存这个图片并修改对应的 slider 数据

轮播图的参考数据结构

```typescript
interface SliderImage {
  id: string;
  link: string;
  metadata: Record<string, unknown>;
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

递交作业内容

1. 源代码
2. 单元测试代码以及单元测试覆盖率(覆盖率请勿提交整个目录，一张图片或一个 text table 即可)
3. API 集成测试案例以及测试结果
4. 简单的框架设计图，以及所有做的假设
5. 涉及的 SQL 的 Schema，注意标注出 Primary key 和 Index 如果有。

其他

- 我们期望不要过度设计，每一个依赖以及每一行代码都有足够充分的理由。

## 加分项

- 逻辑性强的业务框架设计
- 程序具有良好的健壮性
- 缓存
