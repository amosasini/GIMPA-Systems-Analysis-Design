# Patient Appointment Scheduling System

## Context Diagram

The diagram illustrates the interaction between the patient, the appointment scheduling system, and the notification service.

```mermaid
flowchart LR
    Patient[Patient]
    System[Appointment Scheduling System]
    Notification[Notification Service]

    Patient -->|Requests appointment rescheduling| System
    System -->|Sends AppointmentRescheduled event| Notification
    System -->|Displays updated appointment confirmation| Patient
