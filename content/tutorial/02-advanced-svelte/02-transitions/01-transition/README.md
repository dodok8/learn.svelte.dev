---
title: The transition directive
---

요소들이 DOM에 나타나고 사라질때 우아하게 전환함으로써 더 매력적인 유저 인터페이스를 만들 수 있습니다. Svelte에서는`transition` 지시어를 사용하여 이를 매우 쉽게 할 수 있습니다.

먼저, `fade` 함수를 `svelte/transition`에서 임포트합니다.

```svelte
/// file: App.svelte
<script>
	+++import { fade } from 'svelte/transition';+++
	let visible = true;
</script>
```

그리고 `<p>` 요소에 적용합니다.:

```svelte
/// file: App.svelte
<p +++transition:fade+++>
	Fades in and out
</p>
```
