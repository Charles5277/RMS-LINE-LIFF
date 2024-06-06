<script setup lang="ts">
import { ref } from 'vue';
import { Todo, Meta } from 'src/components/models';

defineOptions({
  name: 'IndexPage',
});

const todos = ref<Todo[]>([
  {
    id: 1,
    content: 'ct1',
  },
  {
    id: 2,
    content: 'ct2',
  },
  {
    id: 3,
    content: 'ct3',
  },
  {
    id: 4,
    content: 'ct4',
  },
  {
    id: 5,
    content: 'ct5',
  },
]);

const meta = ref<Meta>({
  totalCount: 1200,
});

console.log('todos', todos.value);
console.log('meta', meta.value);
</script>
