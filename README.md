VueJS Snippets
=======================

<a href="https://twitter.com/@gabrielva" target="_blank">@gabrielva</a>


```cson
'.source.js, .vue':
  'Vue App':
    'prefix': 'vue'
    'body': """
      var ${1:app} = new Vue({
        el: '${2:#app}'
      })
    """
  'Vue Data':
    'prefix': 'vue-data'
    'body': """
      data() {
        return {$1}
      }
    """
  'Vue Extend':
    'prefix': 'vue-extend'
    'body': """
      var ${1:component} = Vue.extend({
        template: '$2'
      });
    """
  'Vue NextTick':
    'prefix': 'vue-nexttick'
    'body': """
      Vue.nextTick(${1:() => {
        $2
      }}${3});
    """
  'Vue Set':
    'prefix': 'vue-set'
    'body': """
      Vue.set($1${2:,'key'}${3:,'value'});
    """
  'Vue Delete':
    'prefix': 'vue-delete'
    'body': """
      Vue.delete($1${2: ,'key'});
    """
  'Vue Directive':
    'prefix': 'vue-directive'
    'body': """
      Vue.directive('${1:my-directive}', () => {
        ${2:// this will be called as `bind` and `update`}
      });
    """
  'Vue Filter':
    'prefix': 'vue-filter'
    'body': """
      Vue.filter('${1:my-filter}', () => {
        ${2:// return processed value}
      });
    """
  'Vue Component':
    'prefix': 'vue-component'
    'body': """
      Vue.component('${1:my-component}', {
        $2
      });
    """
  'Vue Use':
    'prefix': 'vue-use'
    'body': """
      Vue.use($1);
    """
  'Vue Mixin':
    'prefix': 'vue-mixin'
    'body': """
      Vue.mixin($1);
    """
  'Vue Compile':
    'prefix': 'vue-compile'
    'body': """
      Vue.compile('$1');
    """
  'Vue Version':
    'prefix': 'vue-version'
    'body': """
      Vue.version
    """
  'Vue Props':
    'prefix': 'vue-props'
    'body': """
      props: [$1]
    """
  'Vue Props Data':
    'prefix': 'vue-props-data'
    'body': """
      propsData: {
        $1
      }
    """
  'Vue Computed':
    'prefix': 'vue-computed'
    'body': """
      computed: {
        ${1:name}: () => {
          return $2;
        }
      }
    """
  'Vue Methods':
    'prefix': 'vue-methods'
    'body': """
      methods: {
        ${1:name}: () => {
          $2
        }
      }
    """
  'Vue Watch':
    'prefix': 'vue-watch'
    'body': """
      watch: {
        ${1:name}: (val, oldVal) => {
          $2
        }
      }
    """
  'Vue Before Create':
    'prefix': 'vue-before-create'
    'body': """
      beforeCreate() {
        $1
      }
    """
  'Vue Created':
    'prefix': 'vue-created'
    'body': """
      created() {
        $1
      }
    """
  'Vue Before Mount':
    'prefix': 'vue-before-mount'
    'body': """
      beforeMount() {
        $1
      }
    """
  'Vue Mounted':
    'prefix': 'vue-mounted'
    'body': """
      mounted() {
        $1
      }
    """
  'Vue Before Update':
    'prefix': 'vue-before-update'
    'body': """
      beforeUpdate() {
        $1
      }
    """
  'Vue Updated':
    'prefix': 'vue-updated'
    'body': """
      updated() {
        $1
      }
    """
  'Vue Activated':
    'prefix': 'vue-activated'
    'body': """
      activated() {
        $1
      }
    """
  'Vue Deactivated':
    'prefix': 'vue-deactivated'
    'body': """
      deactivated() {
        $1
      }
    """
  'Vue Before Destroy':
    'prefix': 'vue-before-destroy'
    'body': """
      beforeDestroy() {
        $1
      }
    """
  'Vue Destroyed':
    'prefix': 'vue-destroyed'
    'body': """
      destroyed() {
        $1
      }
    """
  'Vue Directives':
    'prefix': 'vue-directives'
    'body': """
      directives: {
        $1
      }
    """
  'Vue Filters':
    'prefix': 'vue-filters'
    'body': """
      filters: {
        $1
      }
    """
  'Vue Components':
    'prefix': 'vue-components'
    'body': """
      components: {
        $1
      }
    """
  'Vue Parent':
    'prefix': 'vue-parent'
    'body': """
      parent: ${1}
    """
  'Vue Mixins':
    'prefix': 'vue-mixins'
    'body': """
      mixins: {
        $1
      }
    """
  'Vue Extends':
    'prefix': 'vue-extends'
    'body': """
      extends: {
        $1
      }
    """
  'Vue Provide':
    'prefix': 'vue-provide'
    'body': """
      provide: {
        ${1:name}: ${2:'value'}
      }
    """
  'Vue Inject':
    'prefix': 'vue-inject'
    'body': """
      inject: [${1:''}]
    """
  'Vue Name':
    'prefix': 'vue-name'
    'body': """
      name: '$1'
    """
  'Vue Delimiters':
    'prefix': 'vue-delimiters'
    'body': """
      delimiters: ['${1:\\$\\{}', '${2:\\}}']
    """
  'Vue Functional':
    'prefix': 'vue-functional'
    'body': """
      functional: ${1:true}
    """
  'Vue Model':
    'prefix': 'vue-model'
    'body': """
      model: {
        prop: '${1:checked}',
        event: '${2:change}'
      }
    """
  'Directives: Vue Text':
    'prefix': 'v-text'
    'body': """
      v-text="${1:message}"
    """
  'Directives: Vue HTML':
    'prefix': 'v-html'
    'body': """
      v-html="${1:html}"
    """
  'Directives: Vue Show':
    'prefix': 'v-show'
    'body': """
      v-show="${1:show}"
    """
  'Directives: Vue If':
    'prefix': 'v-if'
    'body': """
      v-if="${1:condition}"
    """
  'Directives: Vue Else':
    'prefix': 'v-else'
    'body': """
      v-else
    """
  'Directives: Vue Else If':
    'prefix': 'v-else-if'
    'body': """
      v-else-if="${1:condition}"
    """
  'Directives: Vue For':
    'prefix': 'v-for'
    'body': """
      v-for="${1:item} in ${2:items}"
    """
  'Directives: Vue For Index':
    'prefix': 'v-for-index'
    'body': """
      v-for="(${1:item}, ${2:index}) in ${3:items}"
    """
  'Directives: Vue On Event':
    'prefix': 'v-on'
    'body': """
      v-on:${1:click}="${2:callback}"
    """
  'Directives: Vue Short On Event':
    'prefix': 'v-on-short'
    'body': """
      @${1:click}="${2:callback}"
    """
  'Directives: Vue On Click':
    'prefix': 'v-on-click'
    'body': """
      @click="${2:callback}"
    """
  'Directives: Vue Bind':
    'prefix': 'v-bind'
    'body': """
      v-bind:${1:prop}="${2:value}"
    """
  'Directives: Vue Bind Short':
    'prefix': 'v-bind-short'
    'body': """
      :${1:prop}="${2:value}"
    """
  'Directives: Vue Model':
    'prefix': 'v-model'
    'body': """
      v-model="${1:name}"
    """
  'Directives: Vue Pre':
    'prefix': 'v-pre'
    'body': """
      v-pre
    """
  'Directives: Vue Cloak':
    'prefix': 'v-cloak'
    'body': """
      v-cloak
    """
  'Directives: Vue Once':
    'prefix': 'v-once'
    'body': """
      v-once
    """
```



