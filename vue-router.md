# about vue-router

## I want to add page-not-found page

```
const routes = [
{
  path: '*',
  component: PageNotFound
}
];
```
vue3 에서는 아래와 같이 작성해야 한다.

```
const routes = [
{
  path: '/:pathMatch(.*)*',
  component: PageNotFound
}
];
```
