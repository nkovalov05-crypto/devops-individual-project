# My DevOps Project (`nkovalov05`)

Простий вебсервіс на Python, упакований у Docker та розгорнутий на AWS EC2 за допомогою Terraform і GitHub Actions.

## Локальний запуск у Docker

```bash
cd students/nkovalov05
docker build -t nkova05/devops-project:latest .
docker run -d -p 8080:8080 nkova05/devops-project:latest
```

Після запуску сторінка відкривається за адресою `http://localhost:8080`.

## Змінні середовища та секрети GitHub Actions

У репозиторії налаштовані секрети: `DOCKER_USERNAME`, `DOCKER_TOKEN`, `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`, `EC2_SSH_KEY_B64`.