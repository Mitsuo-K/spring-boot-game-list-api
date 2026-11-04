# Spring Boot Game List API

REST API for a catalog of games organized in lists, built during a free Java course in July 2023.

## Endpoints

| Method | Path | Returns |
| --- | --- | --- |
| GET | `/games` | All games, short version |
| GET | `/games/{id}` | One game with full details |
| GET | `/lists` | All game lists |
| GET | `/lists/{listId}/games` | The games in a list, in list order |

## Stack

Java 17, Spring Boot 3.1, Spring Data JPA, H2 in-memory database seeded from `import.sql`.

## Running

`./mvnw spring-boot:run` — the default `test` profile uses H2, with the console at `/h2-console`.
