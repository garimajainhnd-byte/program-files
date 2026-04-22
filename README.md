[program-1 WAP for addition sub mul div using object and classes](#code1)
[program-1 WAP for addition of two distance where each distance is given in m,cm,mm](#code1)
[program-1 WAP for similarly,test the result by creation of object in main class where each distance is given in m,cm](#code1)
[program-1 WAP for similarly for time given in hours,min and seconds](#code1)
[program-1 WAP for time given in hours and miniutes](#code1)
[program-1 WAP for collect the code from internet for any five programs of c language (fact,armstrong,palindrome,fibonacci,pattern)](#code1)
[program-1 WAP for class that is having four meyhod for 1-dimensionalarray](#code1)
[program-1 WAP for  ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
[program-1 WAP for ](#code1)
## Assi-1
```
class Arithmetic {
    int a = 10, b = 5;

    void add() { System.out.println("Add: " + (a + b)); }
    void sub() { System.out.println("Sub: " + (a - b)); }
    void mul() { System.out.println("Mul: " + (a * b)); }
    void div() { System.out.println("Div: " + (a / b)); }

    public static void main(String[] args) {
        Arithmetic obj = new Arithmetic();
        obj.add(); obj.sub(); obj.mul(); obj.div();
    }
}
```

<img width="594" height="185" alt="image" src="https://github.com/user-attachments/assets/681015d1-13aa-4480-b07a-222354312a75" />

## Assi-2
```
class Distance {
    int m, cm, mm;

    Distance(int m, int cm, int mm) {
        this.m = m;
        this.cm = cm;
        this.mm = mm;
    }

    void add(Distance d) {
        int total = (m*1000 + cm*10 + mm) + (d.m*1000 + d.cm*10 + d.mm);

        int m1 = total / 1000;
        int r = total % 1000;
        int cm1 = r / 10;
        int mm1 = r % 10;

        System.out.println(m1 + "m " + cm1 + "cm " + mm1 + "mm");
    }

    public static void main(String[] args) {
        Distance d1 = new Distance(2,50,5);
        Distance d2 = new Distance(1,30,7);
        d1.add(d2);
    }
}
```

<img width="630" height="120" alt="image" src="https://github.com/user-attachments/assets/eee6122d-4d6a-436b-ac78-4b2406f22b61" />

## Assi-3
```
class DistanceTest {
    int m, cm;

    DistanceTest(int m, int cm) {
        this.m = m;
        this.cm = cm;
    }

    void display() {
        System.out.println("Distance: " + m + "m " + cm + "cm");
    }

    public static void main(String[] args) {
        DistanceTest d = new DistanceTest(5, 75);
        d.display();
    }
}
```

<img width="627" height="116" alt="image" src="https://github.com/user-attachments/assets/6a71736e-79ce-4d04-b03e-8ed43be66f2c" />

## Assi-4
```
class TimeFull {
    int h, m, s;

    TimeFull(int h, int m, int s) {
        this.h = h;
        this.m = m;
        this.s = s;
    }

    void display() {
        System.out.println("Time: " + h + "h " + m + "m " + s + "s");
    }

    public static void main(String[] args) {
        TimeFull t = new TimeFull(2, 45, 30);
        t.display();
    }
}
```

<img width="595" height="123" alt="image" src="https://github.com/user-attachments/assets/5fadfad1-a9c5-4c53-afb2-61823f8df17c" />

## ASSI-5
```
class TimeHM {
    int h, m;

    TimeHM(int h, int m) {
        this.h = h;
        this.m = m;
    }

    void display() {
        System.out.println("Time: " + h + " hours " + m + " minutes");
    }

    public static void main(String[] args) {
        TimeHM t = new TimeHM(3, 40);
        t.display();
    }
}
```

<img width="589" height="118" alt="image" src="https://github.com/user-attachments/assets/aaaa9f35-4e45-44b4-8aa2-af296db913e2" />

## Assi-6(a)
```
#include <stdio.h>

int main() {
    int n = 5, fact = 1;
    for(int i = 1; i <= n; i++)
        fact *= i;

    printf("Factorial = %d", fact);
    return 0;
}
```

<img width="677" height="121" alt="image" src="https://github.com/user-attachments/assets/c5d0eae3-0f91-4e60-bd70-cc1cc7a6e5b5" />

6(b)
```
#include <stdio.h>

int main() {
    int n = 153, temp, r, sum = 0;
    temp = n;

    while(n > 0) {
        r = n % 10;
        sum += r*r*r;
        n /= 10;
    }

    if(temp == sum)
        printf("Armstrong Number");
    else
        printf("Not Armstrong");

    return 0;
}
```

<img width="661" height="126" alt="image" src="https://github.com/user-attachments/assets/f6901ef1-a149-4344-be1f-40834166b6be" />

6(c)
```
#include <stdio.h>

int main() {
    int n = 121, rev = 0, temp = n;

    while(n > 0) {
        rev = rev * 10 + n % 10;
        n /= 10;
    }

    if(temp == rev)
        printf("Palindrome");
    else
        printf("Not Palindrome");

    return 0;
}
```

<img width="695" height="119" alt="image" src="https://github.com/user-attachments/assets/470678a8-58c0-472b-a78f-780814619eee" />

6(d)
```
#include <stdio.h>

int main() {
    int n = 10, a = 0, b = 1, c;

    printf("%d %d ", a, b);

    for(int i = 2; i < n; i++) {
        c = a + b;
        printf("%d ", c);
        a = b;
        b = c;
    }

    return 0;
}
```

<img width="657" height="114" alt="image" src="https://github.com/user-attachments/assets/315f7133-45a6-4214-bf3a-28a8b2f2bc31" />

6(e)
```
#include <stdio.h>

int main() {
    for(int i = 1; i <= 5; i++) {
        for(int j = 1; j <= i; j++) {
            printf("* ");
        }
        printf("\n");
    }
    return 0;
}
```

<img width="661" height="216" alt="image" src="https://github.com/user-attachments/assets/66319966-16e2-47c9-96a1-8d56ebc0ab2b" />

## Assi-7
```
class Array1D {
    int arr[] = {10, 20, 30, 40, 50};

    void display() {
        System.out.print("Array: ");
        for(int i : arr)
            System.out.print(i + " ");
        System.out.println();
    }

    void reverse() {
        System.out.print("Reverse: ");
        for(int i = arr.length - 1; i >= 0; i--)
            System.out.print(arr[i] + " ");
    }

    public static void main(String[] args) {
        Array1D obj = new Array1D();
        obj.display();
        obj.reverse();
    }
}
```

<img width="615" height="142" alt="image" src="https://github.com/user-attachments/assets/8ee4b3e7-12c4-43c1-be66-9e09f3bff8dd" />

## Assi-8
```
class MatrixOps {
    int[][] a = {{1,2,3},{4,5,6},{7,8,9}};

    void display() {
        System.out.println("Matrix:");
        for(int i=0;i<3;i++){
            for(int j=0;j<3;j++){
                System.out.print(a[i][j]+" ");
            }
            System.out.println();
        }
    }

    void transpose() {
        System.out.println("Transpose:");
        for(int i=0;i<3;i++){
            for(int j=0;j<3;j++){
                System.out.print(a[j][i]+" ");
            }
            System.out.println();
        }
    }

    void rowSum() {
        for(int i=0;i<3;i++){
            int sum=0;
            for(int j=0;j<3;j++){
                sum += a[i][j];
            }
            System.out.println("Row "+i+" sum: "+sum);
        }
    }

    void colSum() {
        for(int j=0;j<3;j++){
            int sum=0;
            for(int i=0;i<3;i++){
                sum += a[i][j];
            }
            System.out.println("Col "+j+" sum: "+sum);
        }
    }

    public static void main(String[] args) {
        MatrixOps m = new MatrixOps();
        m.display();
        m.transpose();
        m.rowSum();
        m.colSum();
    }
}

```

<img width="589" height="401" alt="image" src="https://github.com/user-attachments/assets/7031e402-890d-4775-90b1-00d0f94d9d1f" />

## Assi-9
```
class A extends Thread {
    public void run() {
        for(int i=1;i<=100;i++)
            System.out.println("A: " + i);
    }
}

class B extends Thread {
    public void run() {
        for(int i=1;i<=100;i++)
            System.out.println("B: " + i);
    }
}

class C extends Thread {
    public void run() {
        for(int i=1;i<=100;i++)
            System.out.println("C: " + i);
    }
}

class ThreadDemo {
    public static void main(String[] args) {
        A t1 = new A();
        B t2 = new B();
        C t3 = new C();

        t1.start();
        t2.start();
        t3.start();
    }
}
```

<img width="599" height="807" alt="image" src="https://github.com/user-attachments/assets/5a7b2328-2289-4d8e-9a84-4297a6fae7de" />

## Assi-10
```
class A extends Thread {
    public void run() {
        for(int i=1;i<=10;i++)
            System.out.println("A: " + i);
    }
}

class B extends Thread {
    public void run() {
        for(int i=1;i<=10;i++)
            System.out.println("B: " + i);
    }
}

class C extends Thread {
    public void run() {
        for(int i=1;i<=10;i++)
            System.out.println("C: " + i);
    }
}

class ThreadJoin {
    public static void main(String[] args) throws Exception {
        A t1 = new A();
        B t2 = new B();
        C t3 = new C();

        t1.start();
        t1.join();

        t2.start();
        t2.join();

        t3.start();
        t3.join();
    }
}
```

<img width="644" height="756" alt="image" src="https://github.com/user-attachments/assets/d950fb82-2792-4936-bb81-60ece7c55e20" />

## Assi-11
```
import javax.swing.*;
import java.awt.event.*;

class AddSwing {
    public static void main(String[] args) {
        JFrame f = new JFrame("Addition");

        JTextField t1 = new JTextField();
        JTextField t2 = new JTextField();
        JTextField t3 = new JTextField();
        JButton b = new JButton("Add");

        t1.setBounds(50,50,100,30);
        t2.setBounds(50,100,100,30);
        b.setBounds(50,150,100,30);
        t3.setBounds(50,200,100,30);

        f.add(t1); f.add(t2); f.add(b); f.add(t3);

        b.addActionListener(e -> {
            int a = Integer.parseInt(t1.getText());
            int b1 = Integer.parseInt(t2.getText());
            t3.setText(String.valueOf(a + b1));
        });

        f.setSize(300,300);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```

<img width="350" height="358" alt="image" src="https://github.com/user-attachments/assets/306cca18-35f4-4f9d-b7b8-e2c3599cc24b" />

## Assi-12
```
import javax.swing.*;
import java.awt.event.*;

class RegistrationForm {
    public static void main(String[] args) {
        JFrame f = new JFrame("Registration");

        JLabel l1 = new JLabel("Name:");
        JTextField t1 = new JTextField();

        JLabel l2 = new JLabel("Email:");
        JTextField t2 = new JTextField();

        JButton b = new JButton("Submit");

        l1.setBounds(50,50,100,30);
        t1.setBounds(150,50,150,30);

        l2.setBounds(50,100,100,30);
        t2.setBounds(150,100,150,30);

        b.setBounds(100,160,100,30);

        f.add(l1); f.add(t1);
        f.add(l2); f.add(t2);
        f.add(b);

        b.addActionListener(e -> {
            System.out.println("Data Submitted: " + t1.getText() + " " + t2.getText());
        });

        f.setSize(400,300);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```

<img width="469" height="353" alt="image" src="https://github.com/user-attachments/assets/e8ee00fe-9761-4e39-8473-e9fc5652bcc9" />

<img width="667" height="135" alt="image" src="https://github.com/user-attachments/assets/d78aa138-366e-4dbd-a192-f1355e12399f" />


## Assi-13
```
import javax.swing.*;
import java.awt.event.*;

class CalculatorSwing {
    public static void main(String[] args) {
        JFrame f = new JFrame("Calculator");

        JTextField t1 = new JTextField();
        JTextField t2 = new JTextField();
        JTextField t3 = new JTextField();

        JButton add = new JButton("+");

        t1.setBounds(50,50,100,30);
        t2.setBounds(50,100,100,30);
        add.setBounds(50,150,100,30);
        t3.setBounds(50,200,100,30);

        f.add(t1); f.add(t2); f.add(add); f.add(t3);

        add.addActionListener(e -> {
            int a = Integer.parseInt(t1.getText());
            int b = Integer.parseInt(t2.getText());
            t3.setText(String.valueOf(a + b));
        });

        f.setSize(300,300);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```

<img width="351" height="358" alt="image" src="https://github.com/user-attachments/assets/729edb2d-c13f-4346-b5e6-2fda6761c066" />

## Assi-14
```
import javax.swing.*;
import java.awt.event.*;

class MatrixSwing {
    public static void main(String[] args) {
        JFrame f = new JFrame("Matrix Addition");

        JTextField a1 = new JTextField();
        JTextField a2 = new JTextField();
        JTextField b1 = new JTextField();
        JTextField b2 = new JTextField();
        JTextField r1 = new JTextField();

        JButton add = new JButton("Add");

        a1.setBounds(50,50,50,30);
        a2.setBounds(110,50,50,30);
        b1.setBounds(50,100,50,30);
        b2.setBounds(110,100,50,30);
        add.setBounds(50,150,100,30);
        r1.setBounds(50,200,100,30);

        f.add(a1); f.add(a2);
        f.add(b1); f.add(b2);
        f.add(add); f.add(r1);

        add.addActionListener(e -> {
            int x1 = Integer.parseInt(a1.getText());
            int x2 = Integer.parseInt(a2.getText());
            int y1 = Integer.parseInt(b1.getText());
            int y2 = Integer.parseInt(b2.getText());

            r1.setText((x1+y1) + " " + (x2+y2));
        });

        f.setSize(300,300);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```

<img width="353" height="363" alt="image" src="https://github.com/user-attachments/assets/a5f9ac03-959a-47f2-866a-8be82e19f660" />

## Assi-15
```
import javax.swing.*;
import java.awt.event.*;

class ShapeButtons {
    public static void main(String[] args) {
        JFrame f = new JFrame("Shapes");

        JButton b1 = new JButton("Circle");
        JButton b2 = new JButton("Rectangle");
        JButton b3 = new JButton("Oval");

        b1.setBounds(50,50,120,30);
        b2.setBounds(50,100,120,30);
        b3.setBounds(50,150,120,30);

        f.add(b1); f.add(b2); f.add(b3);

        b1.addActionListener(e -> System.out.println("Circle Selected"));
        b2.addActionListener(e -> System.out.println("Rectangle Selected"));
        b3.addActionListener(e -> System.out.println("Oval Selected"));

        f.setSize(300,300);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```

<img width="621" height="157" alt="image" src="https://github.com/user-attachments/assets/d141e979-b883-4a85-b1b1-5c7baa266c8e" />

## Assi-16
```
import javax.swing.*;
import java.awt.event.*;

class ShapeButtons {
    public static void main(String[] args) {
        JFrame f = new JFrame("Shapes");

        JButton b1 = new JButton("Circle");
        JButton b2 = new JButton("Rectangle");
        JButton b3 = new JButton("Oval");

        b1.setBounds(50,50,120,30);
        b2.setBounds(50,100,120,30);
        b3.setBounds(50,150,120,30);

        f.add(b1); f.add(b2); f.add(b3);

        b1.addActionListener(e -> System.out.println("Circle Selected"));
        b2.addActionListener(e -> System.out.println("Rectangle Selected"));
        b3.addActionListener(e -> System.out.println("Oval Selected"));

        f.setSize(300,300);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```

<img width="345" height="358" alt="image" src="https://github.com/user-attachments/assets/ac39cd41-2d65-47d0-bef7-dbd0715b2f7c" />

<img width="621" height="157" alt="image" src="https://github.com/user-attachments/assets/b8f177c6-d9d7-4d32-816d-6fb3489a28d4" />


## Assi-17
```
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;

class PaintBrush extends JFrame {
    int x, y;

    PaintBrush() {
        addMouseMotionListener(new MouseMotionAdapter() {
            public void mouseDragged(MouseEvent e) {
                x = e.getX();
                y = e.getY();
                repaint();
            }
        });

        setSize(400,400);
        setTitle("Paint Brush");
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setVisible(true);
    }

    public void paint(Graphics g) {
        g.fillOval(x, y, 10, 10);
    }

    public static void main(String[] args) {
        new PaintBrush();
    }
}
```

<img width="470" height="479" alt="image" src="https://github.com/user-attachments/assets/cc4ec760-2822-47d0-829d-19a09e4728a6" />

## Assi-18
```
class ExceptionDemo {
    public static void main(String[] args) {

        try {
            int a = 10 / 0;
        } catch (Exception e) {
            System.out.println("Arithmetic Exception Occurred");
        }

        try {
            int arr[] = new int[5];
            arr[10] = 20;
        } catch (Exception e) {
            System.out.println("Array Index Out of Bounds");
        }
    }
}
```

<img width="633" height="137" alt="image" src="https://github.com/user-attachments/assets/1469ad7a-9205-49dc-8699-eaa1a91abd5a" />

## Assi-19
```
class AgeException extends Exception {
    AgeException(String msg) {
        super(msg);
    }
}

class TestAge {
    static void checkAge(int age) throws AgeException {
        if(age < 18)
            throw new AgeException("Age must be 18+");
        else
            System.out.println("Valid Age");
    }

    public static void main(String[] args) {
        try {
            checkAge(16);
        } catch (Exception e) {
            System.out.println(e.getMessage());
        }
    }
}
```

<img width="650" height="115" alt="image" src="https://github.com/user-attachments/assets/a720e3fc-40ec-4f17-a8e5-6ef74e9f386d" />

## Assi-20
```
import java.io.*;

class FileHandling {
    public static void main(String[] args) {
        try {
            FileWriter fw = new FileWriter("test.txt");
            fw.write("Hello File Handling");
            fw.close();

            BufferedReader br = new BufferedReader(new FileReader("test.txt"));
            String s;
            while((s = br.readLine()) != null) {
                System.out.println(s);
            }
            br.close();

        } catch(Exception e) {
            System.out.println(e);
        }
    }
}
```

<img width="642" height="123" alt="image" src="https://github.com/user-attachments/assets/f1efb52f-c20f-4304-ae55-33d246c4a909" />

## Assi-21
```
interface A {
    void show();
}

abstract class B {
    abstract void display();
}

class C extends B implements A {
    public void show() {
        System.out.println("Interface Method");
    }

    void display() {
        System.out.println("Abstract Method");
    }
}

class InheritanceDemo {
    public static void main(String[] args) {
        C obj = new C();
        obj.show();
        obj.display();
    }
}
```
<img width="644" height="139" alt="image" src="https://github.com/user-attachments/assets/c5e6d14b-229d-4762-b0eb-fbc9bef79481" />




``````
