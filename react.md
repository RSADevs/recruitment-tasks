# React tasks

## Component with hook

We have one hook `useSampleHook` and one simple component `Sample`.
Please go through the code to see what this code exactly does.

```
const useSampleHook = () => {
    console.log('Test');
}

type ComponentProps = {
    flag?: boolean;
}

const Sample: FunctionComponent<ComponentProps> = ({ flag = true }) => {
    if (flag) {
        return null;
    }
    const hook = useSampleHook();

    return (<h1>Hello World!</h1>)
}
```

Please determine what will be an output of embeding this component inside another one using:

```
<Sample />
```

## Iteration over collection

Given that we have a collection:

```
const items: string[] = ['Foo', 'Bar', 'Baz', 'Foo'];
```

and we want to iterate over this collection to display each of entry in the following way:

```
return (
    <>
        {items.map((item, index) => (
            <div>
                {item}
            </div>
        ))}
    </>
)
```

- What this code is missing?
- Do you know any rules of using it?
