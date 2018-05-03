# vue-dropdowns
A prettier way to display select boxes if you're selecting objects if you're using a v-for on objects.

No special dependencies, no jquery, no bootstrap, just VueJS and CSS goodness.

# Demo
 - [Demo - https://mikerodham.github.io/vue-dropdowns/](https://mikerodham.github.io/vue-dropdowns/)

# Requirements

- [Vue.js](https://github.com/vuejs/vue) `^2.0.0`

# Installation

```shell
$ npm install https://github.com/zOxta/vue-dropdowns/tarball/master
```

# Usage

```html
<dropdown :options="arrayOfObjects" :selected="object" :truncate-selected-option="25" @updateOption="methodToRunOnSelect"></dropdown>

<script>
import dropdown from 'vue-dropdowns';

export default {
        data() {
          return {
            arrayOfObjects: [],
            object: {
              name: 'Object Name',
            }
          }
        },

        components: {
            'dropdown': dropdown,
        },

        methods: {
          methodToRunOnSelect(payload) {
            this.object = payload;
          }
        }
      }
</script>

```

# Todo
- Add different styles to choose from
- Add option to include own styling via json object

# License

[The MIT License](http://opensource.org/licenses/MIT)
