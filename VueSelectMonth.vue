<script>
Vue.component('select-month', {
  data: function () {
    return {
      months: [ {'num':'1','name':'Январь'},
                {'num':'2','name':'Февраль'},
                {'num':'3','name':'Март'},
                {'num':'4','name':'Апрель'},
                {'num':'5','name':'Май'},
                {'num':'6','name':'Июнь'},
                {'num':'7','name':'Июль'},
                {'num':'8','name':'Август'},
                {'num':'9','name':'Сентябрь'},
                {'num':'10','name':'Октябрь'},
                {'num':'11','name':'Ноябрь'},
                {'num':'12','name':'Декабрь'}]
    }
  },
  template: '<select v-model="note.month">
  <option v-for="(month,index) in months" class="form-control" v-bind:value="month.num">
    {{ month.name }}
  </option>
</select>'
})
</script>
