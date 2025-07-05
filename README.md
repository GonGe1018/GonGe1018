# plz FIX THE BAN AI

[@instagram](https://github.com/instagram)
</br>
[@Meta](https://github.com/facebook)
</br>
[@MetaResearch](https://github.com/facebookresearch)

```js
class MetaAI {
  private gpu;

  constructor(GPUs: unknown) {
    // @ts-expect-error: 'this.gpu' is declared but its value is never read.
    this.gpu = GPUs;
  }
  public isBanTarget(userId: string): boolean {
    return Math.random() > 0.5;
  }
}

const ai = new MetaAI(ManyGPUs);
const users = await getUsers();

users.forEach(user => ai.isBanTarget(user.id));
```
