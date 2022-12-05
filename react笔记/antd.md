修改UI组件库中的样式：
1. 找到渲染后的内容，我们去观察它的样式类和相关样式
2. 按照样式类去修改样式，只要保证我们自己写的样式权重高即可「可基于 !important 提高权重」

## antd Form表单
![antd Form表单](images/antd%20Form表单.jpg)

## 
![antd表格render](images/antd%E8%A1%A8%E6%A0%BCrender.jpg)

触发Form表单校验的方式：
1. 前提：提交按钮包裹在`<Form>`中，并且htmlType='submit'
   点击这个按钮，会自动触发Form的表单校验
   表单校验通过，会执行 `<Form onFinish={函数}>` 事件
       函数执行，形参获取的就是表单收集的信息
2. 我们获取Form组建的实例「或者是子组件内部返回的方法」
   基于这些方法，触发表单校验 & 获取表单手机的信息等
   + validateFields
   + getFieldsValue
   + resetFields
   + ….
