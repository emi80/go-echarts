---
id: api
title: API 设计
sidebar_label: API 设计
---

go-echarts 秉承着 API 设计要简洁的原则，对所有图表只提供了下面的接口


### Render(w ...io.Writer)
负责渲染图表，支持传入多个实现了 io.Writer 接口的对象

### Add(arg0 Type0, arg1 Type1, ...)
新增 series，参数由具体图表决定

### AddXAxis(arg0 Type0, arg1 Type1, ...)
新增 X 轴数据，参数由具体图表决定

### AddYAxis(arg0 Type0, arg1 Type1, ...)
新增 X 轴数据，参数由具体图表决定

### Overlap()

### func SetGlobalOptions(options ...globalOptser) *RectChart {}
设置全局配置项

### func SetSeriesOptions(options ...seriesOptser) {}
设置 Series 配置项