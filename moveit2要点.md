1.创建MoveGroupInterface对象，与move_group交互，用于规划和执行轨迹。
    using moveit::planning_interface::MoveGroupInterface;
2.使用lamda进行隐式显示时，采用[]{}()的方式进行，其中
[&]通过引用的方法读取变量，或者调用成员函数改变他的状态。而不写&则意味着将对象直接拷贝到函数内部
{}中写明主要参数，而()表   示立即执行。如果没有最后的()，变量得到的是一个函数对象，而不是return的返回值
对于[](参数){}()的形式，{}前可再加入一个参数，声明传入的参数类型，例如（std：：string text)表示可传入类型为std::string的参数，而(auto text)表示可传入任意形式的参数.