# orm
2019-2-1

根据个人对ORM框架理解的一个简单实现
#
2019-2-5

有如下一个仓库接口：
```java
public interface EntityRepository {

    void sayHello();
}
```

获取该接口的实现类:
```java
public class MyRepositoryFactoryTest {

    @Test
    public void getRepositoryAgent() {

        MyRepositoryFactory factory = new MyRepositoryFactory(null);
        EntityRepository m=factory.getRepositoryAgent(EntityRepository.class);
        m.sayHello();
    }
}
```
