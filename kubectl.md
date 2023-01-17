

## Commands:

#### `kubectl api-resources`
list supported resources
`--api-group=''`
	limit to resources in the specified api group
`-o, --output=''`
	output format  (ok values={`wide`, `name`})
`-sort-by=''`
	how to sort results (ok values = {`name`, `kind`})

**list all api resources**
>  `kubectl api-resources`

#### `kubectl get`
displays one or many resources

**list all pods (ps format):**
>  `kubectl get pods`

**list all deployments**
>  `kubectl get deployments`


#### `kubectl describe TYPE OBJ `
show details for/of specific resource(s)

**get verbose information about a given pod**
>  `kubectl describe pod my-pod`

#### `kubectl scale SCALEABLE_TYPE OBJ`
set a new size for a scaleable type (eg: `deployment`, `statefulset`)
`--replicas=0`
	how many replicas to scale to

**scale a given deployment**
>  `kubectl scale deployment my-deployment --replicas=3` 

