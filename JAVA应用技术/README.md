## JAVA

楼Sir班的，上课讲的基本不考

一定要去看lwm班的PPT

期末考多刷刷往年题

今年三个函数题，第一个考了枚举类，第二个考了Collection，第三个基本类操作，前两题得分率很低。

还有一个程序填空考了IntStream的filter

因为题目集考完就关闭了，所以看不了，只能放代码了

##### 函数题第1题

```java
	add {
		int eval(int x, int y) {
			return x+y;
		}
	},
	sub {
		int eval(int x, int y) {
			return x-y;
		}
	};
```

##### 函数题第2题

```java
	public static ArrayList<String> pick(ArrayList<String> a) {
		for (int i = 0; i < a.size(); i++) {
			for (int j = i+1; j < a.size(); j++ ) {
				if (a.get(i) != null && a.get(j) != null && a.get(j).equals(a.get(i)))
					a.set(j, "#######");
			}
		}
		for (int i = 0; i < a.size(); i++) {
			if (a.get(i).equals("#######")) a.remove(a.get(i));
		}
		a.sort((x, y)->y.compareTo(x));
		return a;
	}
```



##### 函数题第3题

```java
	public double getX() { return x; }
	public double getY() { return y; }
	public void setX(double xx) { x=xx; }
	public void setY(double yy) { y=yy; }
	public Point add(Point p) {
		return new Point(x+p.x,y+p.y);
	}
	Point() { x=0; y=0;}
	Point(double xx, double yy) { x=xx; y=yy;}
	Point(Point p){x=p.x; y=p.y;}
```

