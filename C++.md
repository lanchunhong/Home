# C++

## 基本语法

### 类

```
class Line
{
   public:
      void setLength( double len );
      double getLength( void );
      Line();  // 这是构造函数
      Line(double len);  // 这是带参数的构造函数
      ~Line();  // 这是析构函数声明
 
   private:
      double length;
};
 
// 成员函数定义，包括构造函数
Line::Line(void)
{
    cout << "Object is being created" << endl;
}

Line::Line( double len)
{
    cout << "Object is being created, length = " << len << endl;
    length = len;
}

Line::~Line(void)
{
    cout << "Object is being deleted" << endl;
    delete ptr;
}
```

