# PostgreSQL image
FROM postgres:latest

# Define environment variables
ENV POSTGRES_DB foodie
ENV POSTGRES_USER prod_user
ENV POSTGRES_PASSWORD prod_pw

COPY queries/food.sql /docker-entrypoint-initdb.d/

# Create a volume for PostgreSQL data
VOLUME ["/var/lib/postgresql/data"]
