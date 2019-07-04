# Vue Tailwind Modal

A Vue component that creates a Modal using [Tailwind CSS]([https://](https://tailwindcss.com).

## Project setup

```
npm install --save vue-tailwind-modal
```

or

```
yarn add vue-tailwind-modal
```

## Using the modal

### Installing globally

In your main js file:

``` js
import VueTailwindModal from 'vue-tailwind-modal'
Vue.use(VueTailwindModal);
```

### Using within a component

In your component .vue file

``` js
import VueTailwindModal from 'vue-tailwind-modal'

export default {
  components: {
	VueTailwindModal,
	...
  },
  ...
```

Once installed simply use as any other component:

``` html
<vue-tailwind-modal :showing="true" @close="showModal = false">
<!-- Put your modal content here -->
</vue-tailwind-modal>
```

To hide and show the modal simply pass a boolean to the :showing attribute (true to show, false to hide). 
You can capture the close event using @close to hide the modal (as in the example above) and do further processing.