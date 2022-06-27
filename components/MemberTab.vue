<!-- Please remove this file from your project -->

 <template>
  <v-simple-table  class="elevation-1">
    <template v-slot:default>
      <thead>
        <tr class="header-table">
          <th class="text-left" id="text-table">
            Name
          </th>
          <th class="text-center" id="text-table">
            Team
          </th>
           <th class="text-center" id="text-table">
            Role
          </th>
           <th class="text-center" id="text-table">
            Stastus
          </th>
        </tr>
      </thead>
      <tbody>
        <tr
          v-for="item in desserts"
          :key="item.name"
        >
          <td>{{ item.Name }}</td>
          <td class="text-center" >{{ item.Team }}</td>
          <td class="text-center" >{{ item.Role }}</td>
          <td class="text-center" style="font-weight:bold;">{{ item.Status }}</td>
        </tr>
      </tbody>
    </template>
  </v-simple-table>
</template>  
<script>
  export default {
    data: () => ({
      desserts: [
        {
          Name: 'Sophon',
          Team:'Business Team',
          Role:'Meeting Organizer',
          Status:'Join'
        },
         {
          Name: 'Pongsit',
          Team:'Manager',
          Role:'Role',
          Status:'Join'
        },
      ],
      headers: [
        { text: 'Name', value: 'Name' },
        { text: 'Team', value: 'Team' },
        { text: 'Role', value: 'Role' },
        { text: 'Status', value: 'Status' },
      ],
    }),
  }
</script>
<style>
.v-data-table__wrapper{
    height: auto;
}
#text-table{
    color: #ffffff !important;
    font-size: medium;
}
.main{
  padding: 50px;
}
.header-table{
    background-color:  #45a2db !important;
    border: none;
}
.btn-sumary {
  border: thin solid #45a2db !important ;
  color: #45a2db !important;
}
.elevation-1{
   background-color: #ffffff !important; 
  color: #000000 !important; 
  border: none;
}
.content{
  color: #000000 !important;
  padding: 50px;
}
.status{
    font-weight: bold;
}
.th{
    background-color: #2190bd !important;
     border: none;
}
</style>
