PRJ-EDU-HORARIOS/
│
├── docs/
├── src/
├── tests/
├── docker/
├── scripts/
│
├── .env
├── .gitignore
├── README.md
├── pom.xml
└── package.json


---DOCUMENTOS---

docs/
│
├── c4/
├── requirements/
├── kpi/
└── open-questions/


--- DOCUMENTOS C4---

c4/
│
├── c1-context/
├── c2-containers/
├── c3-components/
└── adr/


---C1 CONTEXT---

c1-context/
│
├── c1-system-context.drawio
├── c1-system-context.png
├── c1-system-context.puml
└── README.md

---C2 CONTAINERS---
c2-containers/
│
├── c2-container-diagram.drawio
├── c2-container-diagram.png
├── c2-container-diagram.puml
└── README.md

---C3 COMPONENTS---

c3-components/
│
├── c3-security-module.drawio
├── c3-schedules-module.drawio
├── c3-inventory-module.drawio
├── c3-reports-module.drawio
├── c3-observations-module.drawio
└── README.md

---           SRC          ---

src/
│
├── modules/
├── shared/
└── main/


---         MODULES        ---

modules/
│
├── security/
├── schedules/
├── inventory/
├── observations/
├── reports/
└── instructors/


---         SEGURITY        ---

security/
│
├── controller/
├── service/
├── repository/
├── entity/
├── dto/
├── mapper/
├── config/
├── middleware/
├── utils/
└── tests/


--- SEGURITY-CONTROLLER  ---

service/
│
├── AuthService.java
├── UserService.java
└── RoleService.java


--- SEGURITY-REPOSITORY ---

repository/
│
├── UserRepository.java
└── RoleRepository.java

--- SEGURITY-ENTITY---

entity/
│
├── User.java
├── Role.java
└── Permission.java


--- SEGURITY - DTO ---

dto/
│
├── LoginDTO.java
├── UserDTO.java
└── TokenDTO.java

--- SEGURITY - UTILS ---

utils/
│
└── jwt/
    ├── JwtProvider.java
    └── JwtUtils.java

--- SCHEDULES ---
schedules/
│
├── controller/
├── service/
├── repository/
├── entity/
├── dto/
├── validators/
├── rules/
├── mapper/
└── tests/

---SCHEDULES-CONTROLLER---

controller/
│
├── ScheduleController.java
├── AvailabilityController.java
└── CalendarController.java

---SCHEDULES-SERVICE---

service/
│
├── ScheduleService.java
├── AvailabilityService.java
├── ValidationService.java
└── AssignmentService.java

---SCHEDULES-REPOSITORY---

repository/
│
├── ScheduleRepository.java
├── TimeSlotRepository.java
└── AvailabilityRepository.java

---SCHEDULES-ENTITY---

entity/
│
├── Schedule.java
├── TimeSlot.java
├── AcademicGroup.java
└── Assignment.java

