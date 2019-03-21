#笔记 ---- 集合
集合：与数组类似，可存放多个对象，但是区别于数组，集合不需要事先规定长度；
##ArrayList （implement List）:
###常用方法：
* 添加
`add()`
* 判断是否存在
`contains()`
* 获取指定位置的对象
`get()`
* 获取指定对象的位置
`indexOf()`
* 删除
`remove()`
* 替换
`set()`
* 获取大小
`size()`
* 转换为数组
`toArray()`
* 添加另一个容器的对象
`addAll()`
* 清空
`clear()`
###List集合遍历
####1、使用for()循环遍历
```
public static void main(String[] args) {
    ArrayList<Integer> list = new ArrayList<>();
    for(int i = 0; i < 10; i++){
        list.add(Integer.valueOf(i));
    }

    for(int i = 0; i<10; i++){
        System.out.println(list.get(i));
    }
}
```
####1、使用迭代器遍历
```
public static void main(String[] args) {
    ArrayList<Integer> list = new ArrayList<>();
    for(int i = 0; i < 10; i++){
        list.add(Integer.valueOf(i));
    }

    //使用迭代器 --- While
    Iterator<Integer> integerIterator = list.iterator();
    while (integerIterator.hasNext()){
        System.out.println(integerIterator.next());
    }

    //使用迭代器 --- for
    for(Iterator<Integer> i = list.iterator(); i.hasNext();){
        System.out.println(i.next());
    }

}
```
####1、使用增强型for()循环遍历
```
public static void main(String[] args) {
    ArrayList<Integer> list = new ArrayList<>();
    for(int i = 0; i < 10; i++){
        list.add(Integer.valueOf(i));
    }

    for (Integer a:list
         ) {
        System.out.println(a);
    }

}
```
##Map集合
键值对，Map<KEY, VALUE>
###注：

* Map存储方式：键值对
* Map内键是唯一的，值可相同

##Set集合
###注：
* set集合内元素不可重复
* 存放是无序的
* 不提供get()方法来获取元素的位置


