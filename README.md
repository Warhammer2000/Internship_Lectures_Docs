InChargeSolution/
├── Core/
│   ├── Entities/               
│   │   ├── Lecture.cs
│   │   └── Mentor.cs
│   ├── Repositories/              
│   │   ├── ILectureRepository.cs
│   │   └── IMentorRepository.cs
│   ├── Results/        
│   │   ├── Result.cs
│   │   └── ResultT.cs
│   └── Services/         
│       ├── ILectureService.cs
│       └── IMentorService.cs

├── Application/
│   ├── Services/                  # Реализации сервисов
│   │   ├── LectureService.cs
│   │   └── MentorService.cs
│   └── DTOs/                  
│       ├── LectureDto.cs
│       └── MentorDto.cs

├── Infrastructure/
│   ├── Persistence/       
│   │   ├── AppDbContext.cs
│   │   └── Configuration/  
│   │       ├── LectureConfiguration.cs
│   │       └── MentorConfiguration.cs
│   ├── Repositories/  
│   │   ├── LectureRepository.cs
│   │   └── MentorRepository.cs
│   ├── Caching/          
│   │   ├── CachingLectureRepository.cs
│   │   └── CachingMentorRepository.cs
│   ├── Logging/                  
│   │   └── SerilogConfiguration.cs
│   └── BackgroundJobs/            
│       └── LectureProcessingJob.cs

├── API/                           # Web API (слой представления)
│   ├── Controllers/          
│   │   ├── LectureController.cs
│   │   └── MentorController.cs
│   ├── Logging/                   
│   │   └── LogMessages.cs
│   ├── Middlewares/              
│   │   ├── GlobalErrorHandlingMiddleware.cs
│   │   └── RateLimitingMiddleware.cs
│   ├── Program.cs               
│   └── appsettings.json          

└── Tests/                         
    ├── UnitTests/                 
    │   ├── LectureServiceTests.cs
    │   └── MentorServiceTests.cs
    └── IntegrationTests/         
        ├── LectureRepositoryTests.cs
        └── MentorRepositoryTests.cs
