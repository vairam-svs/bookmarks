Repository Pattern
CQRS (Command Query Responsibility Segregation) - http://martinfowler.com/bliki/CQRS.html
http://stackoverflow.com/questions/25688292/query-with-repository-pattern
Active Record: entity has both properties and behavior including code to persist.
http://guides.rubyonrails.org/active_record_basics.html
http://www.martinfowler.com/eaaCatalog/activeRecord.html 
Difference between ActiveRecord and DAO: http://stackoverflow.com/questions/6640784/difference-between-active-record-and-dao

http://stackoverflow.com/questions/8550124/what-is-the-difference-between-dao-and-repository-patterns
:::
DAO is an abstraction of data persistence. Repository is an abstraction of a collection of objects.

DAO would be considered closer to the database, often table-centric. Repository would be considered closer to the Domain, dealing only in Aggregate Roots. A Repository could be implemented using DAO's, but you wouldn't do the opposite.

Also, a Repository is generally a narrower interface. It should be simply a collection of objects, with a Get(id), Find(ISpecification), Add(Entity). A method like Update is appropriate on a DAO, but not a Repository - when using a Repository, changes to entities would usually be tracked by separate UnitOfWork.

It does seem common to see implementations called a Repository that are really more of a DAO, and hence I think there is some confusion about the difference between them.


DDD: 
http://domaindrivendesign.org/resources/what_is_ddd
