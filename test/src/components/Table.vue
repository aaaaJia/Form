<template>
    <a-table v-for="item in data" :columns="columns" :data-source="item.result.data" :scroll="{ x: 1500, y: 300 }">
      <template #bodyCell="{ column }">
        <!-- <template v-if="column.key === 'operation'">
          <a>action</a>
        </template> -->
      </template>
    </a-table>
    <!-- <div v-for="item in data">
      {{item.result.data[1].deviceId}}
    </div> -->
  </template>
  <script setup>
  const columns = [
    {
      title: '创建时间',
      width: 200,
      dataIndex: 'time',
      key: 'time',
      fixed: 'left',
    },
    {
      title: '设备ID',
      width: 100,
      dataIndex: 'deviceId',
      key: 'deviceId',
      fixed: 'left',
    },
    {
      title: '0.3um',
      dataIndex: 'P03um',
      key: 'P03um',
      width: 150,
    },
    {
      title: '0.5um',
      dataIndex: 'P05um',
      key: 'P05um',
      width: 150,
    },
    {
      title: '1um',
      dataIndex: 'P1um',
      key: 'P1um',
      width: 150,
    },
    {
      title: '3um',
      dataIndex: 'P3um',
      key: 'P3um',
      width: 150,
    },
    {
      title: '5um',
      dataIndex: 'P5um',
      key: 'P5um',
      width: 150,
    },
    {
      title: '10um',
      dataIndex: 'P10um',
      key: 'P10um',
      width: 150,
    },
    {
      title: '流量',
      dataIndex: 'traf',
      key: 'traf',
      width: 150,
    },
  
  ];
  const data = [
    {
      "message": "success",
      "result": {
          "pageIndex": 0,
          "pageSize": 8,
          "total": 765,
          "data": [
              {
                  "P05um": 6464.4,
                  "traf": 1.88,
                  "P03um": 15068.2,
                  "P5um": 0.0,
                  "P10um": 0.0,
                  "time": "2024-11-07 14:34:00",
                  "P1um": 1331.6,
                  "deviceId": "JC-601P-010",
                  "P3um": 69.8
              },
              {
                  "P05um": 6412.33,
                  "traf": 2.35,
                  "P03um": 14873.83,
                  "P5um": 0.0,
                  "P10um": 0.0,
                  "time": "2024-11-07 14:32:00",
                  "P1um": 1301.0,
                  "deviceId": "JC-601P-010",
                  "P3um": 67.16
              },
              {
                  "P05um": 6327.66,
                  "traf": 2.36,
                  "P03um": 14771.0,
                  "P5um": 0.0,
                  "P10um": 0.0,
                  "time": "2024-11-07 14:30:00",
                  "P1um": 1297.33,
                  "deviceId": "JC-601P-010",
                  "P3um": 74.33
              },
              {
                  "P05um": 6383.83,
                  "traf": 2.35,
                  "P03um": 14976.83,
                  "P5um": 0.5,
                  "P10um": 0.16,
                  "time": "2024-11-07 14:28:00",
                  "P1um": 1327.5,
                  "deviceId": "JC-601P-010",
                  "P3um": 76.0
              },
              {
                  "P05um": 6379.83,
                  "traf": 2.3,
                  "P03um": 14876.83,
                  "P5um": 1.66,
                  "P10um": 0.33,
                  "time": "2024-11-07 14:26:00",
                  "P1um": 1273.33,
                  "deviceId": "JC-601P-010",
                  "P3um": 70.66
              },
              {
                  "P05um": 6313.16,
                  "traf": 2.37,
                  "P03um": 14866.166,
                  "P5um": 0.33,
                  "P10um": 0.0,
                  "time": "2024-11-07 14:24:00",
                  "P1um": 1278.0,
                  "deviceId": "JC-601P-010",
                  "P3um": 71.83
              },
              {
                  "P05um": 6378.0,
                  "traf": 2.36,
                  "P03um": 14892.33,
                  "P5um": 0.0,
                  "P10um": 0.0,
                  "time": "2024-11-07 14:22:00",
                  "P1um": 1279.0,
                  "deviceId": "JC-601P-010",
                  "P3um": 70.33
              },
              {
                  "P05um": 6362.333,
                  "traf": 2.35,
                  "P03um": 14832.5,
                  "P5um": 0.5,
                  "P10um": 0.0,
                  "time": "2024-11-07 14:20:00",
                  "P1um": 1339.66,
                  "deviceId": "JC-601P-010",
                  "P3um": 74.5
              }
          ]
      },
      "status": 200,
      "timestamp": 1731292812255
  }
  
  ];
  // for (let i = 0; i < 100; i++) {
  //   data.push({
  //     key: i,
  //     name: `Edrward ${i}`,
  //     age: 32,
  //     address: `London Park no. ${i}`,
  //   });
  // }
  
  console.log(data["result"])
  </script>