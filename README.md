# Tp-Java

package ma.education.tp5.collections;

import java.util.ArrayList;
import java.util.List;
public class TestList {


           public static void main(String[] args) {

List<Integer> list1= new ArrayList<Integer>();
list1.add(12);
list1.add(23);
list1.add(23);
list1.add(12);
list1.forEach(i-> System.out.println(" element "+i));
                                                   }
                      }





public class TestList {
    public static void main(String[] args) {
List<Integer> list2= Arrays.asList(1,5,6,9,16);
list2.stream().map(i->i*i).filter(i->i>37).forEach(i->
System.out.println(i));

    }  
    
    
}





public class TestList {
    public static void main(String[] args) {
List<Integer> list3= new ArrayList<>();
list3.add(5);
list3.add(10);
list3.add(15);
list3.add(20);
list3.add(2,10);
list3.forEach(i-> System.out.println(i));

    } 



package ma.education.tp5.collections;

import java.util.HashSet;
import java.util.Set;
public class TestSet {
public static void main(String[] args) {
Set<String> set1 = new HashSet<String>();
set1.add("ABC1");
set1.add("ABC2");
set1.add("ABC3");
set1.add("ABC1");
set1.add("ABC4");
set1.add("ABC5");
set1.forEach(i-> System.out.println(i));
}
} // les doublons n'existent pas dans la Set set1 l’ordre d’insertion n’est pas respecté





package ma.education.tp5.collections;

import java.util.Objects;

class Client{
Integer code;
String name;
@Override
public boolean equals(Object o) {
Client client = (Client) o;
return Objects.equals(this.code, client.code) && this.name.equals(client.name);
}
@Override
public int hashCode() {
return code;
}
}

package ma.education.tp5.collections;

import java.util.Set;
import java.util.TreeSet;
public class TestSet {
public static void main(String[] args) {
Set<Integer> set3 = new TreeSet<>();
set3.add(22);
set3.add(11);
set3.add(15);
set3.add(9);
set3.forEach(i-> System.out.println(i));


}
} 






package ma.education.tp5.collections;

class Client implements Comparable{
Integer code;
String name;
public Client(Integer code, String name) {
this.code = code;
this.name = name;
}
@Override
public String toString() {
return "Client{" +
"code=" + code +
", name='" + name + '\'' +
'}';
}
@Override
public int compareTo(Object o) {
Client client = (Client) o;

return -client.code+this.code;
}
}




package ma.education.tp5.collections;

import java.util.Set;
import java.util.TreeSet;
public class TestSet {
public static void main(String[] args) {
Set<Client> set4 = new TreeSet<>();
set4.add(new Client(1,"OMAR"));
set4.add(new Client(3,"SAID"));
set4.add(new Client(2,"HASSAN"));
set4.forEach(i-> System.out.println(i));


}
} 
repository sur github 
 apres l'excution 



