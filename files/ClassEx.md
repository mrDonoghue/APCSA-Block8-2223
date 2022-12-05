## Snippet A
```java
Person ani = new Person("Anakin");
Person ben = new Person("Obi Wan");
ani.setBestFriend(ben);
ben.setBestFriend(ani);
ani.getBestFriend().increaseMoney(3);
```


## Snippet B
```java
Person ani = new Person("Anakin");
Person ben = new Person("Obi Wan");
ani.setBestFriend(ben);
ben.setBestFriend(ani);

ani.setBestFriend(null);
ani.getBestFriend().increaseMoney(100);
```

## Snippet C
```java
Person bezzy = new Person("Jeffrey");
Person alice = new Person("Alice");
Person customer = alice;
Person seller = bezzy;

customer.decreaseMoney(20);
seller.increaseMoney(20);
```

## New method in Main.java

For any remaining snippets, assume the following method has been added to `Main.java`.
```java
public static void monetaryTransaction(Person seller, Person customer, double price) {
    customer.decreaseMoney(price);
    seller.increaseMoney(price);
}
```

## Snippet D
```java
Person im = new Person("Tony");
im.increaseMoney(1000);
Person cap = new Person("Steve");
cap.increaseMoney(100);
Person ws = new Person("Bucky");
ws.increaseMoney(50);
im.setBestFriend(cap);
cap.setBestFriend(im);

im.decreaseMoney(100);
cap.increaseMoney(100);
cap.setBestFriend(bucky);
Main.monetaryTransaction(cap, cap.getBestFriend(), 30);
Main.monetaryTransaction(bucky, im.getBestFriend(), 50);
```


## Snippet E
```java
Person a = new Person("A");
Person b = new Person("B");
Person c = new Person("C");
c.setBestFriend(a);
a.setBestFriend(c);
b.setBestFriend(a);
c = a;
a = b;
a.setBestFriend(c.getBestFriend());
monetaryTransaction(b, c.getBestFriend(), 30);
```

