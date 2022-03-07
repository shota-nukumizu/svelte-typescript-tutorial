# Svelte✕TypeScriptチュートリアル

SvelteとTypeScriptで簡単なTodoアプリを開発してみる

# インストール

以下のコマンドを入力して、Svelte✕TypeScriptの環境構築を行う

```
npx degit sveltejs/template svelte-app
cd svelte-app
npm i
npm run dev
```

# Todoタスクの設定

まずは以下のコードを書いていく。

`src/types/todo.type.ts`(新規作成)

```ts
// 基本的にはタスク名と完了したかどうかを設定する
export type TodoType = {
    id: number
    name: string
    completed: boolean
}
```

`src/Todo.svelte`(新規作成)

```svelte
<script lang="ts">
    import type { TodoType } from '../src/types/todo.type'

    export let todo:
</script>
```

# 参考サイト

[TypeScript support in Svelte(MDN Web docs)](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/Svelte_TypeScript)