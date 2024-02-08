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
 size++; }  } }
 
