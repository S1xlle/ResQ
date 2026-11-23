# 🚨 ResQ – AI-Powered Emergency Assistance & Community Response Platform

ResQ is an API-driven platform that helps citizens report community incidents (road damage, flooding, electrical hazards...) and helps administrators and response teams resolve them.

> ⚠️ Educational prototype for simulated community incidents. It does not replace official emergency services.

## 🔄 How it works
1. A **Citizen** submits an incident with a description, photo and map location.
2. **AI** suggests a category, priority, summary and department, and detects duplicates.
3. The **Administrator** reviews it, approves it and assigns a **Response Team**.
4. The team updates progress and uploads resolution photos.
5. Everyone receives **real-time notifications** and **emails**; the dashboard shows statistics.

## 👥 User Roles
| Role | Main actions |
|---|---|
| Citizen | Report incidents, track progress, receive notifications |
| Administrator | Review incidents & AI analysis, assign teams, dashboard, reports |
| Response Team | View assignments, update progress, upload resolution photos |

## 🛠️ Technologies
- **Backend:** ASP.NET Core Web API, C#, Entity Framework Core, JWT, ASP.NET Core Identity
- **Database:** Microsoft SQL Server (ResQDB)
- **Frontend:** ASP.NET Core MVC, HTML, CSS, Bootstrap 5, JavaScript, Chart.js
- **Real-time:** SignalR
- **Testing:** Swagger, Postman, xUnit

## 🌐 External APIs
- **AI API** – incident classification, priority, summary, department, duplicates
- **Leaflet + OpenStreetMap + Nominatim** – interactive maps and geocoding
- **Brevo** – email notifications

## 🏗️ Architecture
`ResQ.API` · `ResQ.Application` · `ResQ.Domain` · `ResQ.Infrastructure` · `ResQ.Web` · `ResQ.Tests`

## 📁 Documentation
Project documents are in the `Docs` folder. Daily progress is in [Progress.md](Progress.md).

## 🔐 Security
API keys and secrets are stored in User Secrets / environment variables and are never committed to this repository.
