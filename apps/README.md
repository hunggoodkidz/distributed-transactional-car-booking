
### This is MICROSERVICE AUTO SCALE

distributed-transactional-car-booking/
│
├── docker/                     # File docker-compose, init scripts DB/Redis
│   └── docker-compose.yml
│
├── apps/
│   └── api/                    # NestJS backend project
│       ├── src/
│       │   ├── main.ts
│       │   ├── app.module.ts
│       │   ├── common/         # Redis, exceptions, interceptors
│       │   │   └── redis/
│       │   │        └── redis.module.ts
│       │   ├── modules/
│       │   │   ├── users/
│       │   │   ├── cars/
│       │   │   └── bookings/
│       │   └── config/         # TypeORM config, environment loader
│       │
│       ├── .env.example
│       └── tsconfig.json
│
├── .gitignore
├── package.json
└── README.md