# React Bascis

### Component Defination with propes

```

iimport { ReactNode } from "react"
//defining the structure of propes with optional children
interface GreetProps{
    name:string,
    lastName:string,
    children?:ReactNode
}

export default function Greet({name,lastName,children}:GreetProps){
    return <>
        <h1>Hi {name} {lastName}</h1>
        {children}
    </>
}
```

### passing props

```
<Greet name="APJCR" lastName="jadhav">
        {/* children */}
        <h1>compenent childerns Asgs</h1>
      </Greet>
      <Greet name="APJCR" lastName="Patil"/>
```

### Renderning List

```
function MyList() {

    const names=["APJ","APJCR","JADHVA"];
    //map in seprate line as best practice
    const namesList=names.map((name)=> <h2>{name}</h2>);

  return (
    <div>
        {
            namesList
        }
    </div>
  )
}
```
