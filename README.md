## Java Programing






### this()와 this.의 차이


```markdown
class ConstructExample{
   int x ;
  ConstructExample(String a){
      this(1);
      System.out.println("생성자 호출입니다");
   }
   ConstructExample(int B){
       System.out.println("A");
   }
   public void setX(int x){this.x = x;}
   public int getX(){
      return x;
   }

   public static void main(String[] args){
      ConstructExample a = new ConstructExample("H");
      int n = a.getX();
      System.out.println(n);
   }
}

1. this()는 같은 클래스 내에서 서로 다른 생성자를 호출할 때 쓰인다.
- ConstructExample(String a){생략}에서 this(1)를 사용하는 부분이 있는데 
- 여기서는 자기자신이 아닌 int 형을 매개변수로 받는 ConstructExample(int B){생략}을 호출하는 것 이다.
2. this.은 public void setX(int x){this.x = x;}의
- global 변수인 int x와 매개변수로 받은 x를 구분지어주기 위하여 사용한다.
즉 SetX(int x)의 매소드에서 this.x는 글로벌 변수 x이다.

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/sueunal/Java/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
