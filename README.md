```python
from dataclasses import dataclass


@dataclass
class SoftwareEngineer:
    name: str = "Abunassyr"
    role: str = "Software Engineer"
    location: str = "Milky Way → Solar System → Earth → Asia → Kazakhstan → Almaty"

    bio: str = (
        "Yo, I'm Abunassyr. I'm a Software Engineer who builds, solves problems, "
        "and turns ideas into reliable, working software."
    )

    contacts: dict[str, str] = {
        "telegram": "https://t.me/itzddos",
        "github": "https://github.com/itzddos",
        "email": "mailto:ddosmukhambetov@gmail.com",
    }

    languages = ["Rust", "Python", "SQL", "HTML", "CSS"]
    frameworks = ["Django", "FastAPI"]
    backend = ["REST APIs", "PostgreSQL", "MySQL", "Redis", "Celery"]
    automation = ["RPA", "Selenium", "Workflow Automation", "Scripting"]
    infrastructure = ["Git", "Docker", "Linux", "CI/CD", "Unit Testing"]
    ai = ["PyTorch", "TensorFlow", "Machine Learning", "AI Engineering", "Prompt Engineering"]
    networking = ["CCNA", "Routing & Switching", "VLANs", "Network Security"]

    @property
    def classified(self) -> dict[str, str | None]:
        """Internal information. Access is logged."""
        return {
            "coffee_level": "CRITICAL",
            "sleep": None,
            "bugs": "It's a feature.",
            "salary": "********",
            "production_secrets": "DM for details, XD",
        }


engineer = SoftwareEngineer()
```
