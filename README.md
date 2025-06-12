# Python OOP and Package 🐍

Dự án này chứa các bài tập và ví dụ về Lập trình Hướng Đối tượng (Object-Oriented Programming) trong Python, bao gồm các khái niệm cơ bản đến nâng cao.

## 📋 Mục lục

- [Giới thiệu](#giới-thiệu)
- [Nội dung học](#nội-dung-học)
- [Cấu trúc Project](#cấu-trúc-project)
- [Yêu cầu hệ thống](#yêu-cầu-hệ-thống)
- [Cách sử dụng](#cách-sử-dụng)
- [Các khái niệm chính](#các-khái-niệm-chính)

## 🎯 Giới thiệu

Repository này được tạo ra để học và thực hành các khái niệm lập trình hướng đối tượng trong Python. Từ những khái niệm cơ bản như Classes và Objects đến những chủ đề nâng cao như Inheritance, Abstract Classes, và Iterator Pattern.

## 📚 Nội dung học

### 1. Classes và Objects (Classes.ipynb)
- Định nghĩa Class và Object
- Constructor (`__init__`)
- Access Modifiers (Public, Private)
- Encapsulation
- Aggregation
- Composition

### 2. Inheritance (Inheritance.ipynb)
- Kế thừa cơ bản
- Method Overriding
- Super() function
- Abstract Base Classes (ABC)
- Multiple Inheritance

### 3. Data Structures (LinkedList.ipynb, List-Class.ipynb)
- Cài đặt Linked List
- Iterator Pattern
- Custom List implementations

### 4. Advanced Concepts (Iterator.ipynb)
- Iterator Protocol
- Generator functions
- Custom iterators

### 5. Real-world Examples (OOP_Python.ipynb, OOP_Python_1.ipynb)
- Pizza Store Pattern
- Practical OOP applications

## 📁 Cấu trúc Project

```
Python_Oop_and_Pakage/
├── Classes.ipynb           # Khái niệm cơ bản về Classes
├── Inheritance.ipynb       # Kế thừa và đa hình
├── LinkedList.ipynb        # Cài đặt Linked List
├── List-Class.ipynb        # Custom List class
├── Iterator.ipynb          # Iterator pattern
├── OOP_Python.ipynb       # Ví dụ thực tế
├── OOP_Python_1.ipynb     # Ví dụ bổ sung
└── README.md              # File này
```

## 💻 Yêu cầu hệ thống

- Python 3.9.12 hoặc cao hơn
- Jupyter Notebook
- Các thư viện cần thiết:
  - `abc` (Abstract Base Classes)
  - `math` (Mathematical functions)

## 🚀 Cách sử dụng

1. **Clone repository:**
   ```bash
   git clone https://github.com/QuyDatSadBoy/Python_Oop_and_Pakage.git
   cd Python_Oop_and_Pakage
   ```

2. **Mở Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

3. **Chạy từng notebook theo thứ tự:**
   - Bắt đầu với `Classes.ipynb` để học các khái niệm cơ bản
   - Tiếp tục với `Inheritance.ipynb` để hiểu về kế thừa
   - Thực hành với các file còn lại

## 🔑 Các khái niệm chính

### Classes và Encapsulation
```python
class Cat:
    def __init__(self, name):
        self.__name = name  # Private attribute
    
    def get_name(self):
        return self.__name
```

### Inheritance
```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def computeArea(self):
        pass

class Circle(Shape):
    def __init__(self, radius):
        self.__radius = radius
    
    def computeArea(self):
        return self.__radius * self.__radius * math.pi
```

### Data Structures
```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None
```

### Iterator Pattern
```python
class MyIterator:
    def __iter__(self):
        return self
    
    def __next__(self):
        # Implementation here
        pass
```

## 📝 Ví dụ thực tế

Repository bao gồm một ví dụ thực tế về **Pizza Store System** minh họa việc áp dụng OOP trong thực tế:

```python
def prepare():
    print("1. Prepare ingredient for making NY Style Pizza")
    print("Tossing dough")
    print("Adding sauce")
    print("Adding topping: Grated Reggiano cheese")

def bake():
    print("2. Bake for 25 minutes at 150 oC")

def cut():
    print("3. Cutting the pizza into diagonal slices")

def box():
    print("4. Place pizza in official PizzaStore box")
```

## 🤝 Đóng góp

Nếu bạn muốn đóng góp cho dự án này:
1. Fork repository
2. Tạo branch mới (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Tạo Pull Request

## 📞 Liên hệ

- GitHub: [@QuyDatSadBoy](https://github.com/QuyDatSadBoy)
- Repository: [Python_Oop_and_Pakage](https://github.com/QuyDatSadBoy/Python_Oop_and_Pakage)

## 📄 License

Dự án này được phân phối dưới MIT License. Xem file `LICENSE` để biết thêm chi tiết.

---

⭐ Nếu repository này hữu ích, hãy give một star nhé! ⭐
