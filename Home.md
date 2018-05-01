Welcome to the Calculating-Collections-Time wiki!

array list: no order and can contain duplicate best for insertion element

linked list: follow insertion order & contain duplicate nest for add and removing element


import java.util.*;
public class HelloWorld{

    public static void main(String args[])
{
List<Integer> al =  new ArrayList<Integer>();
List<Integer> ll =  new  LinkedList<Integer>();
doTimings("Arraylist",al);
doTimings("LinkedList",ll);

}
private static void doTimings(String type, List<Integer> list){

for(int i=0;i<1E5;i++){
list.add(i);
}

long start=System.currentTimeMillis();

for(int i=0;i<1E5;i++){
list.add(i);
}

for(int i=0;i<1E5;i++){
list.add(i);
}

long end =System.currentTimeMillis();

System.out.println("Time Take: " + (end- start)+ "ms for" + type);
}

}
