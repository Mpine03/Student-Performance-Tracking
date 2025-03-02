C4Component
  Container(API, "EduTracker API", "Backend - Node.js/Java")

  Component(AuthService, "Authentication Service", "Handles login and security")
  Component(TrackingService, "Tracking Service", "Manages student performance data")
  Component(ReportsService, "Reports Service", "Generates academic reports")

  API -> AuthService : User authentication
  API -> TrackingService : Stores and retrieves student performance
  API -> ReportsService : Generates reports for teachers/parents
