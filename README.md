# quarkus-greeting project

This project uses [Quarkus](https://quarkus.io/), the Supersonic Subatomic Java Framework.

## Running the application in dev mode

Run the application in dev mode to enable live coding:

```bash
./mvnw compile quarkus:dev
```

Once the server has started, request the endpoint in another terminal:

```bash
curl -w "\n" http://localhost:8080/hello
```

Browse to `http://localhost:8080` to see the index page.

When in dev mode, you can also browse to `http://localhost:8080/q/dev/` to view configuration parameters and extensions.

Type `CTRL+C` to stop the application.

## Packaging and running the application

Package the application:

```bash
./mvnw package
```

This will produce a file called `quarkus-run.jar` file in the `target/quarkus-app/` directory.

The dependencies are stored in the `target/quarkus-app/lib/` directory.

The application is now runnable using `java -jar target/quarkus-app/quarkus-run.jar`.

