#### 题目：设计一个简单的图形系统，包含以下类：

1. 抽象类：Shape（图形）

​    \- 属性：name（图形名称，私有）

​    \- 构造方法：初始化name

​    \- 抽象方法：area()（计算面积）、perimeter()（计算周长）

​    \- 普通方法：display()（显示图形名称、面积和周长，使用封装访问name）

2. 接口：Resizable（可调整大小）

​    \- 方法：resize(double scale)（按比例缩放图形）

3. 类：Circle（圆形）继承Shape并实现Resizable

​    \- 属性：radius（半径，私有）

​    \- 构造方法：初始化name和radius

​    \- 实现area()和perimeter()方法

​    \- 实现resize(double scale)方法，按比例缩放半径

4. 类：Rectangle（矩形）继承Shape

​    \- 属性：length（长，私有）、width（宽，私有）

​    \- 构造方法：初始化name、length和width

​    \- 实现area()和perimeter()方法

5. 类：Square（正方形）继承Rectangle

​    \- 构造方法：初始化name和side（边长），调用父类的构造方法（将length和width都		设为side）

6. 在main方法中测试：

​    \- 创建一个Circle对象，计算并显示其面积和周长

​    \- 调整Circle的大小（放大2倍），再次显示

​    \- 创建一个Rectangle对象，计算并显示其面积和周长

​    \- 创建一个Square对象，计算并显示其面积和周长