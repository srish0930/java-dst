# java-dst
//prepend method
java single linked list 
public class linked_list{
private node header;
private node lastnode;
int size;
public linked_list {
header = new Node(null);
lastnode = header; }

public void prepend( Integer data) {
 Node n = new Node(data);
 if(size == 0) {
 header.next = n;
 lastnode =  n; 
 size++; }
 else {
 Node temp = header.next;
 header.next=n;
 n.next=temp;
 size++; }  } 

 public int getSize() {
 return size; }
 public String toString() {
 Node n = header.next;
 String temp = "" ;
 while(n!= null) {
 temp  = temp + n.data + " ";
 n=n.next;
 }
 return temp; } }
 public class main {
 public static void main(String args[]) {
 LinkedList list = new LinkedList();
  list.prepend(1);
  list.prepend(2);
  list.prepend(3);
  list.prepend(4);
  System.out.println(list);
  System.out.println(list.getSize);
  } }
 
