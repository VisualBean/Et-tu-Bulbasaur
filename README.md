# Et tu, Bulbasaur? An engineering case

You are a software engineer working on a new project for a client who is a big fan of both Pokemon and Shakespeare. The client has asked you to create a RESTful API that fetches information about a specific Pokemon and returns its description in Shakespearean language. The API should be containerized using Docker and should include appropriate unit tests and documentation.

## Task

* Use the PokeAPI (https://pokeapi.co/) to fetch information about a specific Pokemon
  * `https://pokeapi.co/api/v2/pokemon-species/{id or name}/` has `flavor_text` that could be interresting
* Use the Fun Translations API (https://funtranslations.com/api/shakespeare) to translate the Pokemon's description into Shakespearean language
  * There's an aggressive rate limiter in place. Are there ways you could work around this limitation?
* Create a RESTful API that takes a Pokemon name or ID as a parameter and returns the Pokemon's information, including its Shakespearean description
* Containerize the API using Docker and ensure that the container can be easily spun up and accessed
* Write unit tests for the API to ensure its functionality
* Provide clear documentation for the API, including instructions on how to set up and use the container, as well as an overview of the API's endpoints and parameters.

### Boilerplate

**We do not** expect a fully functioning application. It is ok to stub parts of the application in order to focus on other aspects that you think show of your skillset better.

**We do not** expect you to use more than a day on the task. The assignment creates a base of discussion for the interview.

**Tip:** Don't waste time on setting up a huge project from scratch. Find a suitable boilerplate and work from that.

* `dotnet new webapi` can get you started quickly with the API
* `ENTRYPOINT ["dotnet", "myapi.dll"]` should help you with docker.
