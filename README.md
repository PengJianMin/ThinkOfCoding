# ThinkOfCoding

+ 实例（占据内存空间，如变量）、类型（抽象概念）、值（抽象概念），理解好这三者的区别和关系。
+ class相当于规制了一种数据类型，并没有占据内存空间，只有用它实例化的变量才会占据内存空间（用到了才会占据内存）
+ 变量本质上是一块内存区域。变量的值的变化实质是指在该内存区域的电位变化。
+ 有的变量是直接放值，有的是间接放值。
+ 类型可以分为三大类：值类型（【内存保存】的层面）、指针类型（【内存地址】层面）、引用类型（【介于内存地址和内存保存内容】两个层面之间。）
+ “访问”指的是使用对象、方法的人能否读取到值、能否使用这个功能的权限，而不是指对象能否访问自己的数据和方法。并且，这个权限和当前代码所在的位置、区域有关。
+ Java没有指针，只有引用的理解：除了基本类型的变量直接保存的是“值”，用于数组和类实例化的变量保存的是“地址值”，地址值需要通过new命令产生，再指派给该变量，这种间接性便有了“引用”的意味。
+ 从另一个角度来看，就是JAVA不去考虑变量本身的地址值，因为我们需要的值都存在了别的地方，通过引用的方式和变量产生关联，不用太关心变量本身在内存中的位置。但是其他类型的语言，变量本身就是保存我们需要的值，所以我们要关注这个变量的内存地址，也就是指针。
+ static静态 这个概念是和动态是相对的。动态指每个类生成的一堆实例是各不相同的，它们各有自己的内存地址和字面值，并且申请内存地址是有随机性的，所以便有了一种动态的含义在里边。因此，静态修饰的变量就是指该变量或者方法不需要申请实例内存就可以使用（但是还是需要有类内存），再往下延伸，就是不需要实例化就能调用，即类就可以直接调用。所以，没有static修饰的也叫作实例的私有变量，有static修饰的也叫类变量，由所有实例共享。
+ 对象和基本数据类型的区别，基本数据类型比如整型是被共享的，具体去看 a=1 和 b=1，实际上都是1这个值在保存在堆内存中，a和b保存的是同一个堆内存的地址，它们指向了同一个地方，这样一来就可以节省内存空间。但是对象不同，每一个对象都开辟在堆内存中，a=new obj() , b= new obj(), 是属于两个不同的对象，a和b保存的是不同堆内存的地址。所以从这一点上去看，值传递和引用传递本质上都是地址传递。
