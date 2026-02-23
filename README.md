# SmartCampus_HelpDeskAi
Smart Campus Helpdesk API is a Django REST Framework–based backend system where students can raise tickets and admins can manage them. It supports JWT authentication, CRUD operations, pagination, filtering, ordering, and search, providing a clean and efficient campus issue-management solution.

#Core Features
-Django project + modular app structure
-PostgreSQL database integration
-Ticket model with required fields
-CRUD operations for tickets
-JWT Authentication (Login + Refresh)
-Admin session login (via Django admin)
-Pagination for ticket listing
-Filtering by category and status
-Ordering by priority and created_at
-Search by title or description
-Clean, professional code structure

#PROJECT STRUCTURE
SmartCampusHelpdesk/

│── tickets/
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   ├── urls.py
│── manage.py

#Database
The project uses PostgreSQL:
DATABASES = {
    "default": {
        "ENGINE": "django.db.backends.postgresql",
        ...
    }
}

#Ticket Model Fields
-id
-title
-description
-category (classroom / hostel / network)
-priority (low / medium / high)
-status (open / in-progress / closed)
-created_at
-updated_at

#Authentication Flow
-User username & password se login karega
-JWT access & refresh token generate honge
-Protected APIs ke liye Authorization header me token bhejna hoga
-Admin users session login bhi use kar sakte hain

#Conclusion
This project is fully functional, scalable, and follows proper REST API standards.
