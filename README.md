# 이진트리 (binary tree)  <br><br>

 <br><br><br>
 ## 이진트리란
 각각의 노드가 최대 두 개의 자식 노드를 가지는 트리 자료 구조이다.
 <br><br>
 자식 노드를 각각 왼쪽 자식 노드 와 오른쪽 자식 노드 라고 한다.
 
 ![image](https://user-images.githubusercontent.com/114748816/227129450-df575330-6d54-4e89-959e-88163596a411.png)

### 트리에서의 위치에 따라
루트(root) 노드: 최상위 노드 <br>
단말(말단, terminal) 노드 / 잎(leaf) 노드: 자식 노드가 없는 노드 <br>
내부(internal) 노드: 자식이 1개 이상 있는 노드 <br>
![image](https://user-images.githubusercontent.com/114748816/227130668-bfe9e992-5a44-4568-b55d-1e73590e4f06.png) <br><br>

### 노드 사이의 관계 관점에서
부모(parent) 노드: 어떤 노드의 직접적인 상위 노드 <br>
자식(child) 노드: 어떤 노드의 직접적인 하위 노드 <br>
선조(ancestor) 노드: 어떤 노드의 상위 노드들 <br>
후손(descendent) 노드: 어떤 노드의 하위 노드들 <br>
형제(sibling) 노드: 같은 부모를 갖는 노드 <br><br>

### 부모 노드
 ![image](https://user-images.githubusercontent.com/114748816/227135545-31575f67-5a88-440f-8cff-fe63b017055d.png)
<br><br>

### 자식 노드
8을 제외한 모든 노드가 상위 노드를 가지므로 8을 제외한 전체 노드가 자식 노드이다. <br>
![image](https://user-images.githubusercontent.com/114748816/227135278-74ef73ef-34fc-4f59-87d1-f5f0c88ffd0f.png) <br><br>

### 선조 노드
![image](https://user-images.githubusercontent.com/114748816/227135110-fb1b3956-5579-40cd-87ef-6aedfd14ed13.png) <br><br>

### 후손 노드
![image](https://user-images.githubusercontent.com/114748816/227390781-862328b4-9fc4-4643-9795-3aeb52b44755.png) <br><br>

### 형제 노드
![image](https://user-images.githubusercontent.com/114748816/227391337-e956daff-d13b-4eab-87a0-fa953e48a8cf.png) <br><br>

<br><br><br><br>
## 기초적인 자바코드
```java
public class node {
	
	int data;
	private node left;
	private node right;
	
	
	public node(int data, node left, node right	) { 
		this.data = data;
		this.left = left;
		this.right = right;
		}
	
	public int getData() {
		return data;
	}
	
	public void setData(int data) {
		this.data = data;
	}
	
	public node getLeft() {
		return left;
	}
	
	public node getRight() {
		return right;
	}
	
	public void setRight(node right) {
		this.right = right;
	}
}
```
