1. **프로젝트 설치**
    ```bash
    git clone https://github.com/dgseo1101/fastapi_layerd_architecture.git
    cd fastapi_layered_architecture
    ```

2. **의존성 설치**
    ```bash
    poetry shell
    poetry install

    (poetry-shell) alembic revision --autogenerate -m "init"
    (poetry-shell) alembic upgrade head
    ```

3. **프로젝트 실행**
    ```bash
    python run_server_local.py --env dev

    or 

    docker build --tag (tag) -f _docker/Dockerfile . 
    docker run --add-host host.docker.internal:host-gateway -p 8000:8000 (tag)
    ```
