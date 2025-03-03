# JPA(Java Persistence API) DevNote

## Entitymanager

JPA에서 제공하는 핵심 **인터페이스**로, 데이터베이스와 애플리케이션 간의 **상호작용을 관리하는 역할**을 합니다. 쉽게 말해, EntityManager는 JPA에서 **데이터베이스 작업을 수행하기 위해 사용되는 객체**이다.

## Persistenc Context(영속성 컨텍스트)

JPA에서 메모리 역할을 하는 공간으로, 엔티티를 관리하며서 해당 객체를 데이터베이스와 동기화하는 작업을 한다.

## Transaction(트랜잭션)

데이터베이스 작업의 일관성(Consistency)과 무결성(Integrity)을 보장하기 위해 관련된 작업들을 하나의 논리적 단위로 묶는 개념이다. JPA에서 트랜잭션은 엔티티에 대한 데이터 변경작업(CRUD)이 데이터베이스에 반영되거나 취소(Rollback)되는 과정을 제어한다.

트랜잭션은 일반적으로 ACID 원칙에 따라 작동한다.

- A (Atomicity): 작업들이 모두 성공하거나 모두 실패해야 한다.
- C (Consistency): 트랜잭션 완료 후 데이터의 무결성이 보장된다.
- I (Isolation): 각 트랜잭션은 서로 독립적으로 실행된다.
- D (Durability): 트랜잭션이 성공하면 결과가 영구적으로 반영된다.
