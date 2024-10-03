# The Courses and documents

Links to courses, API, frameworks, specifications, best practice, project management technics.

## SQL

Database Structure and Design Tutorial </br>
**https://www.lucidchart.com/pages/database-diagram/database-design**

What is a Database Model </br>
**https://www.lucidchart.com/pages/database-diagram/database-models**

Entity-Relationship Diagram Symbols and Notation </br>
**https://www.lucidchart.com/pages/ER-diagram-symbols-and-meaning**

### Postgres

PSW: postgres </br>
**Installation Directory:**</br>
C:\Program Files\PostgresSQL\16<br/>
**Server Installation Directory:**<br/>
C:\Program Files\PostgresSQL\16<br/>
**Data Directory:**<br/>
C:\Program Files\PostgresSQL\16\data<br/>
**Database Port:**<br/>5432<br/>
**Database Superuser:**<br/> postgres<br/>
**Operating System Account:**<br/> NT AUTHORITY\NetworkService<br/>
**Database Service:**<br/>postgresql-x64-16<br/>
**Command Line Tools Installation Directory:**<br/>C:\Program Files\PostgresSQL\16<br/>
**PgAdmin4 Installation Directory:**<br/> 
C:\Program Files\PostgresSQL\16\pgAdmin 4
<br/>
**Stack Builder Installation Directory:**<br/> 
C:\Program Files\PostgresSQL\16<br/>
**Installation Log:** <br/>C:\Users\alexkurylovich\AppData\Local\Temp\install-postgresql.log<br/>
**Run psql command:**<br/>
Env vars: Files\PostgreSQL\16\bin;C:\Program Files\PostgreSQL\16\lib<br/>
psql -U postgres<br/>
psql -U postgres -h localhost dvdrental<br/>
psql -d dvdrental -U postgres -W<br/>
\c <db-name><br/>
**PostgresSQL Sample Database:**<br/>
**https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/**<br/>
DVD rental Database simple study: <br/>
**https://www.kaggle.com/code/fetchii/dvd-rental-database-simple-study** <br/>
Dvdrental databases workshop:<br/>
**https://nuitrcs.github.io/databases_workshop/sql/part1.html**<br/>
COPY film_unknown(film_id, title, description, release_year, language_id, actor_id, film_category_id, length, special_features, fulltext)
FROM 'C:\temp\film_unknown.csv'
DELIMITER ','
CSV HEADER;

SELECT * 
FROM 
  film_unknown
INNER JOIN category 
  ON film_unknown.film_category_id = category.category_id;

Export:<br/>
film_id,title,description,release_year,language_id,actor_id,film_category_id,length,special_features,fulltext
133,Chamber Italian,A Fateful Reflection of a Moose And a Husband who must Overcome a Monkey in Nigeria,2006,,,,117,{Trailers},chamber':1 'fate':4 'husband':11 'italian':2 'monkey':16 'moos':8 'must':13 'nigeria':18 'overcom':14 'reflect':5
384,Grosse Wonderful,A Epic Drama of a Cat And a Explorer who must Redeem a Moose in Australia,2006,,,1,49,"{""Behind the Scenes""}",'australia':18 'cat':8 'drama':5 'epic':4 'explor':11 'gross':1 'moos':16 'must':13 'redeem':14 'wonder':2
8,Airport Pollock,A Epic Tale of a Moose And a Girl who must Confront a Monkey in Ancient India,2006,,1,,54,{Trailers},'airport':1 'ancient':18 'confront':14 'epic':4 'girl':11 'india':19 'monkey':16 'moos':8 'must':13 'pollock':2 'tale':5
98,Bright Encounters,A Fateful Yarn of a Lumberjack And a Feminist who must Conquer a Student in A Jet Boat,2006,,2,1,73,{Trailers},'boat':20 'bright':1 'conquer':14 'encount':2 'fate':4 'feminist':11 'jet':19 'lumberjack':8 'must':13 'student':16 'yarn':5
1,Academy Dinosaur,A Epic Drama of a Feminist And a Mad Scientist who must Battle a Teacher in The Canadian Rockies,2006,2,,,86,"{""Deleted Scenes"",""Behind the Scenes""}",'academi':1 'battl':15 'canadian':20 'dinosaur':2 'drama':5 'epic':4 'feminist':8 'mad':11 'must':14 'rocki':21 'scientist':12 'teacher':17
2,Ace Goldfinger,A Astounding Epistle of a Database Administrator And a Explorer who must Find a Car in Ancient China,2006,3,,2,48,"{Trailers,""Deleted Scenes""}",'ace':1 'administr':9 'ancient':19 'astound':4 'car':17 'china':20 'databas':8 'epistl':5 'explor':12 'find':15 'goldfing':2 'must':14
3,Adaptation Holes,A Astounding Reflection of a Lumberjack And a Car who must Sink a Lumberjack in A Baloon Factory,2006,4,3,,50,"{Trailers,""Deleted Scenes""}","'adapt':1 'astound':4 'baloon':19 'car':11 'factori':20 'hole':2 'lumberjack':8,16 'must':13 'reflect':5 'sink':14"
4,Affair Prejudice,A Fanciful Documentary of a Frisbee And a Lumberjack who must Chase a Monkey in A Shark Tank,2006,5,4,3,117,"{Commentaries,""Behind the Scenes""}",'affair':1 'chase':14 'documentari':5 'fanci':4 'frisbe':8 'lumberjack':11 'monkey':16 'must':13 'prejudic':2 'shark':19 'tank':20
5,African Egg,A Fast-Paced Documentary of a Pastry Chef And a Dentist who must Pursue a Forensic Psychologist in The Gulf of Mexico,2006,1,1,1,130,"{""Deleted Scenes""}",'african':1 'chef':11 'dentist':14 'documentari':7 'egg':2 'fast':5 'fast-pac':4 'forens':19 'gulf':23 'mexico':25 'must':16 'pace':6 'pastri':10 'psychologist':20 'pursu':17
6,Agent Truman,A Intrepid Panorama of a Robot And a Boy who must Escape a Sumo Wrestler in Ancient China,2006,1,1,1,169,"{""Deleted Scenes""}",'agent':1 'ancient':19 'boy':11 'china':20 'escap':14 'intrepid':4 'must':13 'panorama':5 'robot':8 'sumo':16 'truman':2 'wrestler':17
7,Airplane Sierra,A Touching Saga of a Hunter And a Butler who must Discover a Butler in A Jet Boat,2006,1,1,1,62,"{Trailers,""Deleted Scenes""}","'airplan':1 'boat':20 'butler':11,16 'discov':14 'hunter':8 'jet':19 'must':13 'saga':5 'sierra':2 'touch':4"
9,Alabama Devil,A Thoughtful Panorama of a Database Administrator And a Mad Scientist who must Outgun a Mad Scientist in A Jet Boat,2006,1,1,1,114,"{Trailers,""Deleted Scenes""}","'administr':9 'alabama':1 'boat':23 'databas':8 'devil':2 'jet':22 'mad':12,18 'must':15 'outgun':16 'panorama':5 'scientist':13,19 'thought':4"
10,Aladdin Calendar,A Action-Packed Tale of a Man And a Lumberjack who must Reach a Feminist in Ancient China,2006,1,1,1,63,"{Trailers,""Deleted Scenes""}",'action':5 'action-pack':4 'aladdin':1 'ancient':20 'calendar':2 'china':21 'feminist':18 'lumberjack':13 'man':10 'must':15 'pack':6 'reach':16 'tale':7
11,Alamo Videotape,A Boring Epistle of a Butler And a Cat who must Fight a Pastry Chef in A MySQL Convention,2006,1,2,2,126,"{Commentaries,""Behind the Scenes""}",'alamo':1 'bore':4 'butler':8 'cat':11 'chef':17 'convent':21 'epistl':5 'fight':14 'must':13 'mysql':20 'pastri':16 'videotap':2


### Java

JUnit 5 User Guide<br/>
https://junit.org/junit5/docs/current/user-guide/<br/>
Wiremock<br/>
https://www.mocklab.io/blog/<br/>
Which Java HTTP client should I use in 2024<br/>
https://www.wiremock.io/post/java-http-client-comparison<br/>
https://reflectoring.io/comparison-of-java-http-clients/<br/>
A Guide to OkHttp<br/>
https://www.baeldung.com/guide-to-okhttp<br/>
Intro to Feign<br/>
https://www.baeldung.com/intro-to-feign<br/>
The settings.xml File in Maven<br/>
https://www.baeldung.com/maven-settings-xml<br/>
How to Kill a Java Thread<br/>
https://www.baeldung.com/java-thread-stop


### Python

enter python3<br/>
help()<br/>
modules<br/>
q<br/>
import os, sys; print(os.path.dirname(sys.executable))<br>
quit()

### Spring

Spring Microservices in Action<br/>
https://github.com/wuyichen24/spring-microservices-in-action.git<br/>
What Is a Spring Bean?<br/>
https://www.baeldung.com/spring-bean<br/>
Spring @Component Annotation<br/>
https://www.baeldung.com/spring-component-annotation<br/>
@Component vs @Repository and @Service in Spring
https://www.baeldung.com/spring-component-repository-service<br/>
Field injection is not recommended<br/>
https://blog.marcnuri.com/field-injection-is-not-recommended

### JPA

Spring Data JPA<br/>
https://docs.spring.io/spring-data/jpa/docs/current/reference/html/#jpa.sample-app.finders.strategies<br/>
Data Access<br/>
https://docs.spring.io/spring-boot/docs/current/reference/html/howto.html#howto.data-access<br/>
Database initialization<br/>
https://docs.spring.io/spring-boot/docs/1.1.0.M1/reference/html/howto-database-initialization.html<br/>
Spring Data JPA<br/>
https://docs.spring.io/spring-data/jpa/docs/current/reference/html/#repositories<br/>
Hibernate / JPA Joined Table Inheritance Example<br/>
https://www.javaguides.net/2018/11/hibernate-jpa-joined-table-inheritance-example.html<br/>
Guide to JPA with Hibernate - Relationship Mapping<br/>
https://stackabuse.com/a-guide-to-jpa-with-hibernate-relationship-mapping/<br/>
Problems with Hibernate One-To-Many<br/>
https://medium.com/interleap/problems-with-hibernate-one-to-many-and-their-solutions-8f32af216b95<br/>
Problems with Hibernate One-To-Many<br/>
https://www.baeldung.com/entity-to-and-from-dto-for-a-java-spring-application<br/>
Using ModelMapper<br/>
https://www.baeldung.com/java-modelmapper<br/>
Auto-Generated<br/>
https://www.baeldung.com/jpa-get-auto-generated-id<br/>
Inheritance Mapping<br/>
https://www.baeldung.com/hibernate-inheritance<br/>
Show Hibernate/JPA SQL Statements from Spring Boot<br/>
https://www.baeldung.com/sql-logging-spring-boot<br/>
Spring Boot With H2 Database</br>
https://www.baeldung.com/spring-boot-h2-database<br/>

### MyBatis

What is MyBatis?<br/>
https://mybatis.org/mybatis-3/<br/>
Mybatis-spring-boot<br/>
https://mybatis.org/spring-boot-starter/<br/>
MyBatis with Spring<br/>
https://www.baeldung.com/spring-mybatis<br/>

### SWAGGER

http://localhost:8080/swagger-ui/#/ - v3/<br/>
http://localhost:8080/v3/api-docs<br/>
Spring App using Springfox<br/>
https://dev.to/smartyansh/introduction-to-springfox-48ng<br/>
Swagger2 Configuration<br/>
https://howtodoinjava.com/swagger2/swagger-spring-mvc-rest-example/#swagger2-config<br/>

### Angular

https://github.com/bbachi/angular-java-example<br/>
How To Develop and Build Angular App With Java Backend<br/>
https://medium.com/bb-tutorials-and-thoughts/how-to-develop-and-build-angular-app-with-java-backend-87fb603c6e17<br/>
Local<br/>
src/main/ui<br/>
npm start<br/>
spring boot: http://localhost:8080/h2-console/login.do?jsessionid=5d764566141607df9bc6710461bb3372<br/>
ui: http://localhost:4200/<br/>

### MAC

vm_stat | perl -ne '/page size of (\d+)/ and $size=$1; /Pages\s+([^:]+)[^\d]+(\d+)/ and printf("%-16s % 16.2f Mi\n", "$1:", $2 * $size / 1048576);'<br/>
/usr/libexec/java_home -V
Azure<br/>
https://portal.azure.com/?quickstart=true#blade/Microsoft_Azure_Resources/QuickstartCenterBlade<br/>
https://clickup.com/teams/project-management?utm_source=natural-intelligence&utm_medium=cpc&utm_campaign=nat_cpc_am_nnc_acq_trial_all-devices_cpc_lp_x_all-departments_x&utm_content=BjJSWzl0uI<br/>
Alex Kurylovich<br/> 
alex.v.kurylovich@gmail.com, MkavCup1122!






