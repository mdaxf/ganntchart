Gantt is a pure js library to create a gantt chart for the tasks, order. it also supplies the capability to adjust the time, duration through drag and drop. 

<img src="gantt.png" />

Sample code to use it:

<code>
    <div id="productionline_gantt_data" class="gantt_area" style="width:100%; height:100%;" ondragenter="return" ondrop="return" ondragover="return "></div>

    <script>
    productionlinegantt = new Gantt("#productionline_gantt_data", resources,tasks,{
      header_height: 50,
        column_width: 30,
        step: 20,
        view_modes: ['Quarter Day', 'Half Day', 'Day', 'Week', 'Month'],
        bar_height: 40,
        bar_corner_radius: 3,
        arrow_curve: 5,
        padding: 10,
        view_mode: 'Half Day',   
        date_format: 'YYYY-MM-DD',
        custom_popup_html: null,
      xoffset: 0,
      setindex: 'yes',
      showactual: 'no',
      resourccolumnwidth:200,
      resourcechange: 'yes',
      resourcetype: 'line',
      weekend: '0,6',	
      start: start,
      end: end,	
      outofworkingtime: '0-4,20-24',
      on_date_change: function(task, start, end) {

        },
      on_click: function (task) {

        },
      on_resource_change: function(task,oldresource,newresource){

      },
      on_gantt_completion_render: function(gantt){


        });	  

      }


      }  	
      );
    </script>
  </code>
