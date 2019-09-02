# AlevelTestQuestions
(Sample test questions for self-control)

## Databases
- Relational and NoSql databases?
- CAP theory
- Relations in relational DB?
- Normal forms ( enough 3 )
- [ACID](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/Databases/ACID.md)
- Indexes and constraints
- Transactions ( what is it and transaction isolation levels )
- How does JOIN work?
- Basic CRUD queries
- [Group By, Order By, Having By](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/Databases/GroupByOrderByHaving.md) 
- SQL Server query execution pipeline

## .NET Section Common
- What is framework?
- [What is the difference between class and object?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/ClassAndObject.md)
- [Reference VS Value types](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/ReferenceVsValueTypes.md "Reference VS Value types")
- Nullable types
- Boxing/Unboxing
- Methods of Object class
- [What is the difference between string and String?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/stringAndString.md "В чём разница между string и String")
- [Why do we need to determine Equals and GetHashCode?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/EqualsGetHCode.md)
- What is Hash and for what purpose?
- Shallow Vs Deep Copy ( how to implement Deep copy )
- What is auto-properties and how it works?
- Implicit and explicit casts
- Readonly vs Const
- Operator typeof vs *Object.GetType()
- What the difference between is and as
- What is assembly and from which parts consist of?
- What is OOP? Do we really need it?
- OOP vs Functional paradigm 
- OOP principles with examples
- [What are an abstract class and interface and what is the difference in using?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/AbstractClassAndInterface.md "Абстрактные классы & Интерфейсы")
- What can have an abstract class and interface?
- [How does Virtual modifier work?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/Virtual.md)
- How does NEW modifier work?
- [Overloading?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/Overloading.md)
- [Overriding?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/Overriding.md)
- How does CLR resolve which version of virtual method in hierarchy to call?
- Composition vs Inheritance
- How to wrap external libraries during direct using? ( design pattern Adapter, please have a look )
- [How does delegate and event work?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/DelegateAndEvent.md)
- What is the difference between Delegate and Event? ( you must know how to write your own event )
- Which design pattern was taken for Events implementation in .Net? ( Publish/ Subscribe )
- Can Interface be substituted by Delegate and vice versa?
- What is Generic and why do we need it?
- Generic constraints
- [Generics in interfaces?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/GenericInterfaces.md)
- [Generics in delegates?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/GenericDelegates.md)
- Variation in Generic parameters
- Immutable types in .net
- How does type string work in .NET?
- [Try catch finally ?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/TryCatchFinally.md)
- How does using work and  IDisposable interface?
- Garbage collector and how it works?
- [Collections](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/Collections.md "Коллекции")
- Generic vs Non-generic
- What is LINQ?
- [Fluent and Query syntax](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/FluentAndQuerySyntax.md "Синтаксис запросов и синтаксис методов в LINQ")
- [Deffered execution of LINQ queries](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/DeferredExecutionOfLinqQuery.md "Отложенное выполнение запроса LINQ")
- [What is the difference between IEnumerable and IQueryable?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionCommon/IEnumerableVsIQueryable.md)
- Task asynchronous programming model VS Threads
- How does CLR Thread Pool works?
- Basic mechanisms of synchronization in .NET Threading
- SOLID, KISS, DRY
- Design patterns by GOF ( prepare 1-2 for which type of pattern: creational, structural, behavioral)

## .NET Section WEB
- [YOU SHOULD DEFINITELY UNDERSTAND WHAT HAPPENS WHEN YOU TYPE SOMETHING IN URL address and press ENTER](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionWeb/URLAddressAndPressEnter.md)
- What is MVC and how does it work?
- What is the difference between MVC/MVP/MVVM?
- What is the difference between MVC and Web API?
- Application lifecycle
- Http Request lifecycle
- HttpHandlers and HttpModules
- HTTP Verbs and Headers
- Sessions
- Cookies
- Action Filters
- Routing
- ModelBinders
- What is the difference between ASP .NET and .NET Core?
- Javascript ( this and how bind it to the object, hoisting, functional and prototype inheritance, closures, such bullshit like undefined and types in javascript )

## .NET Section MVC and Web API
- [What is MVC? draw a diagram?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionMvcAndWebApi/MVC.md)
- What is WebApi? Give some examples.
- [What is the RESTFULL API?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionMvcAndWebApi/RESTFULLAPI.md)
- What is Razor?
- [What is a PartialView? What is PartialView used for?](https://github.com/ArtemenkoArt/AlevelTestQuestions/blob/master/NetSectionMvcAndWebApi/PartialView.md)
- What is ChildAction?
- What is section?
- What is a Viewbag?
- On the first page, you filled in 10 fields, then you went to a new page. You need to use the information from these 10 fields on the new page. How to transfer information between two requests? Give the maximum of options?
- How to ensure field validation in MVC? How to provide server validation in MVC?
- What is routing? Where can you add routes?
- What types of queries do you know?
- What is the status code? What is the status code used for?
- What is model binding?
- What filters in MVC do you know? What can they be used for? Give examples of the use of filters.
- What is MVC Pipline? Describe what is happening with the request as detailed as possible.
- Why use layered architecture?
- What HTML helper's do you know? What can HTML helper's be used for?
- Why use HTML helper's? Can you do without them?
