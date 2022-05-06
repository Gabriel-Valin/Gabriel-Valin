# USE CASE: README by Gabriel Valin

> ## Data
* Request Fake People to get his informations.
* Code: 
```
axios.get('https://fake-people.com/gabriel-valin')
  .then((response) => {
    console.log(response.data);
  });
```
> ## Output
```
{
  firstName: 'gabriel',
  lastName: 'valin',
  dateBorn: "1999-07-30",
  nationality: "Brazilian",
  favoriteLang: "Javascript/Typescript",
  stack: ["Node.JS", "React", "React Native", "Laravel"],
  contact: {
    email: "gabrielvalincontato@gmail.com",
    linkedin: "https://www.linkedin.com/in/gabriel-valin-dev/",
    twitter: "@gvt3ch"
  }
}
```

> ## Student Data Access

```
class StudentRepository {
  constructor (private readonly entity: Entity<Student>) {}

  public async (name: string) {
    const findStudent = await this.entity.find(name)

    if (!findStudent) return new NoContentError();

    return {
      student: true,
      college: "Faculdade de Tecnologia de Botucatu - FATEC"
    }
  }
}
```

> ## Component Profile

<div align="center" style="display: flex; justify-content: space-between; align-items: center;">
  <img style="border-radius: 50%" src="https://pbs.twimg.com/profile_images/1522262022171332609/PS9NScRu_400x400.jpg">
  <div align="left">
    <strong>Name: </strong> <p>Gabriel Valin</p>
    <strong>Date Born: </strong> <p>30/07/1999</p>
    <strong>Email: </strong> <p>gabrielvalincontato@gmail.com</p>
    <strong>Nationality: </strong> <p>Brazilian 🇧🇷</p>
    <strong>College: </strong><p>Faculdade de Tecnologia de Botucatu - FATEC</p>
  </div>
</div>

<div align="center" style="display: flex; justify-content: center; align-items: center;">
  <a href="https://www.linkedin.com/in/gabriel-valin-dev/">
    <img width="60px" height="60px" src="https://cdn-icons-png.flaticon.com/512/145/145807.png">
  </a>
  <a href="https://twitter.com/gvt3ch" style="margin: 80px 20px 0 20px">
   <img width="60px" height="60px" src="https://cdn4.iconfinder.com/data/icons/social-media-icons-the-circle-set/48/twitter_circle-512.png">
  </a>
  <a href="https://gabrielvalin-dev.vercel.app">
    <img width="60px" height="60px" src="https://assets.vercel.com/image/upload/q_auto/front/favicon/vercel/180x180.png">
  </a> 
</div>
