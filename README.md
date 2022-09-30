<h1 align="center">Doggy App</h1>

<br/>
<div align="center">
<img src=client/src/images/default-dog.png width="200px" atl="imagenotfound"/>
</div>
<br/>
<br/>
This is the repo for Doggy App.
Doggy App is a SPA (Single Page Application) that allows you to search and find information about dog breeds.
Allows you to get close and know their temperaments, life expectancy, weight and average height.

<h2 align="center">Develop of Doggy App</h2>

## API REST consumer

Doggy App is based on a database obtained by the API: <a src="https://thedogapi.com">https://thedogapi.com</a>, as their page says, this is a public service API all about Dogs, free to use for make Fance new App, Website or Service.

## API Reference

### Dogs

```http
  GET /dog
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |

Get particular dog with their id

```http
  GET /dog/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |

Get a particular dogs with their names (here you can receive one or more dogs that meet that name)

```http
  GET /dog?name=${name}
```

| Query  | Type     | Description                          |
| :----- | :------- | :----------------------------------- |
| `name` | `string` | **Required**. name of items to fetch |

### Temperaments

```http
  GET /temp
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |

#### Get particular temperament with their id

```http
  GET temp/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |
