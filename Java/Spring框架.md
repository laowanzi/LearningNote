**1. Spring 到底是如何管理对象的**

我们使用 Spring 的时候，大部分其实都是在使用 Spring 的核心容器功能。

Spring 的容器功能就是通过 BeanFactory 和对应的子类各种 xxxContext 去存储管理对象。

这个知识点是 Spring 发展至今一直没有变化的核心知识。

**2. Spring 注入对象的方式和对应原理**

当 Spring 成为对象容器后，它本身最重要的目的就是要去对系统中各种类进行对象注入。而工作中最常见的问题，就是 Spring 注入对象的各类问题。

也因此，广泛了解 Spring 注入对象的各类方式，从而能更加灵活地运用 Spring，深入理解注入对象的对应原理，从而能顺利无误地使用 Spring，就是我们深入学习 Spring 的重要目标。

**3. Spring 是如何管理对象之间的依赖关系的**

除了使用完整对象的注入以外，工作中，我们还需要考虑对被注入对象属性的动态修改，可能还想要动态地注册新的 Bean 对象等等。

而要做到这些，我们就必须去了解 Spring 是如何管理对象之间的依赖关系的。

**4. AOP 的实现原理以及对其的内部使用**

AOP 在 Spring 项目中被广泛用于权限、错误处理以及日志追踪等关键场景。

尤为重要的是，Spring 项目中的所有相关[数据库事务](https://www.zhihu.com/search?q=数据库事务&search_source=Entity&hybrid_search_source=Entity&hybrid_search_extra={"sourceType"%3A"article"%2C"sourceId"%3A"472022475"})，也都是通过 AOP 来管理和传播的。

所以对 AOP 的学习也颇为重要。

**5. Spring 的扩展点有哪些以及如何做**

很多时候，我们需要把公司的一些内部框架和系统嫁接到 Spring 中。为了减少开发成本，就要自定义一套完整的 Spring 扩展，比如：[自定义注解](https://www.zhihu.com/search?q=自定义注解&search_source=Entity&hybrid_search_source=Entity&hybrid_search_extra={"sourceType"%3A"article"%2C"sourceId"%3A"472022475"})、自定义配置类等。

想做到这些，就必须知道 Spring 有哪些扩展点，可以做什么扩展以及怎么做扩展。

**6. Spring MVC 的体系和重要类的作用**

哪怕现在大家都使用 SpringBoot 了，但是，只要我们在用 SpringBoot 的 Web 功能，其实就是在和 SpringBoot 背后内置的 Spring MVC 打交道。

Spring MVC 本身有一套复杂的体系，从请求到响应，有一套完整复杂的流程。只有了解这些流程和 Spring MVC 的体系，我们才能顺畅使用 Spring MVC，去解决 Web 项目中各种看起来很奇怪的问题以及作出新的扩展功能，比如，项目中的国际化出现的各种乱码问题，统一错误处理问题等。

**7. Spring Boot 是如何自动配置好类的**

Spring Boot 本身就是以 Spring 作为对象容器，以 Spring MVC 实现 Web 功能的一套缝合框架。学习了 Spring 和 Spring MVC 之后，我们就理解了 Spring Boot 绝大部分功能。

但是，Spring Boot 是如何把 Spring 中的各个组件缝合在一起的？其中重要的思想就是自动配置。

所以，学习了 Spring Boot 的自动配置，我们就能从头到尾完整的了解 Spring Boot 的整体体系结构和相关对象管理流程。

提取出学习内容后，强烈建议大家学习中记下我们的笔记和思考，并定期复习。

**说明一下**：除了上述知识点，有一些知识点我没说，例如：Spring MVC 中我并没有提及拦截器，也没有提及Spring Boot 中常用的各种注解。

之所以没说，是因为这些内容，是 Spring 必须内容，你绕不开他们。而我提及的这些，则是 Spring 学习中，大家经常不知所措，也不知道要学的那些重要内容。

Spring Boot 核心作用

* 起步依赖
* 自动配置
* 端点监控













































