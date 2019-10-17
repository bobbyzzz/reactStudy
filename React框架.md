

## React框架

## 一.React的入门

##### 1.React的基本认识

- 英文官网 : https://reactjs.org/
- 中文官网 : https://doc.react-china.org/

##### 2.介绍描述

- 用于构建用户界面的JavaScript库(只关注于View)
- 由Facebook开源

##### 3.React的特点

- Declarative(声明式编码)
- Component-Based(组件化编码)
- Learn Once, Write Anywhere(支持客户端与服务器渲染)
- 高效
- 单项数据流

##### 4.React高效的原因

- 虚拟DOM , 不会先直接操作DOM,而是会在内部生成虚拟DOM树
- Diff算法 , 最小化页面重绘

## 二.React的基本使用

- 1. 相关js库
  
  - react.js React的核心库
  - react-dom.js 提供操作DOM的react扩展库
  - babel.js 解析JSX语法代码转化为纯JS语法代码的库
  
- 2. Hello React 效果

  ![Snipaste_2019-09-14_22-36-57](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-14_22-36-57.png)

-  3.调试工具

  -  [React Developer Tools.crx](调试工具\React Developer Tools.crx) 

-  4.元素渲染

  - ##### 计时器案例

  - ##### React 只更新它需要更新的部分

  - React DOM 会将元素和它的子元素与它们之前的状态进行比较，并只会进行必要的更新来使 DOM 达到预期的状态。

  - 尽管每一秒我们都会新建一个描述整个 UI 树的元素，React DOM 只会更新实际改变了的内容

  - 效果

  ![Snipaste_2019-09-14_23-09-09](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-14_23-09-09.png)

- 5.组件&props

  - 1.简单组件(没有状态的组件)
  - 2.复杂组件(类组件)
  - 3.对props进行校验 (prop-types)
    - 设置props默认值
      - static defaultProps = {   }
    - 设置props输入格式
      - 组件.propTypes = {  key:PropTypes.string.isRequired  }

- 6.state和生命周期

  - 1.效果

    - ![Snipaste_2019-09-15_23-38-13](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-15_23-38-13.png)

  - 2.props和state的区别

    - state: 组件自身内部可变化的数据

    * props: 从组件外部向组件内部传递数据, 组件内部只读不修改

  - 3.组件的生命周期

    - 初始化阶段

      - 1. ```
           constructor
           ```

      - 2. ```
           componentWillMount
           ```

      - 3. ```
           render
           ```

      - 4. ```
           componentDidMount
           ```

    - 更新阶段

      - 1.shouldComponentUpdate
      - 2.componentWillUpdate
      - 3.render
      - 4.componentDidUpdate

    - 卸载阶段

      - 1.componentWillUnmount

    - 解决组件接受新的props时,获取不到外部的props

      - ```
        componentWillReceiveProps: function(nextProps){  console.log(nextProps)  }
        ```

- 7.事件处理&ref

  - 效果
  - ![Snipaste_2019-09-15_00-54-34](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-15_00-54-34.png)
  - ref

- 8.条件渲染

  - 切换Login和Register组件

- 9.列表渲染

  - es6 map函数

- 10.todoLIst案例

  - ![Snipaste_2019-09-15_10-20-57](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-15_10-20-57.png)

- 11.表单

  - 阻止事件默认

- 12.react-cli

  - 效果1:![Snipaste_2019-09-17_01-16-54](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-17_01-16-54.png)

- 13.简书项目

  - 技术栈 es6+webpack+react全家桶(不涉及到flux)+react-ui

  - 1.首页

    - ![Snipaste_2019-09-17_01-19-18](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-17_01-19-18.png)

  - 2.专题分类详情

    - 1.最新分类

      ![Snipaste_2019-09-17_01-20-15](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-17_01-20-15.png)

    - 2.最新收录

      - ![Snipaste_2019-09-17_01-22-11](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-17_01-22-11.png)

    - 3.热门

      - ![Snipaste_2019-09-17_01-22-28](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-17_01-22-28.png)

  - 3.文章详情

    - ![Snipaste_2019-09-17_01-23-10](C:\Users\Administrator\Desktop\react\assets\Snipaste_2019-09-17_01-23-10.png)
