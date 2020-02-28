<template>
  <div class>
    <div class="container">
      <div class="col-md-4 offset-md-4 mb-3 mt-3">
        <p>Number of visitors by blog</p>
      </div>
      <div class="row">
        <div class="col-md-4 col-sm-12">
          <div class="p-3 Unique box_bgcolor">
            <p class="box_title">Unique blog visitors</p>
            <h2>{{blogVisitor}}</h2>
            <div class="btn-blog">
              <button type="button" class="btn">Past 7 Days</button>
              <button type="button" class="btn">Past 30 Days</button>
            </div>
          </div>
          <div class="box_bgcolor Visitors mt-5 p-3">
            <p class="box_title">Visitors who completed a CTA</p>
            <p>
              <vue-svg-gauge
                :start-angle="-90"
                :end-angle="90"
                :value="3"
                :separator-step="0"
                :min="0"
                :max="10"
                :gaugeColor="[{ offset: 0, color: '#7480FF'}, { offset: 100, color: '#69C8D5'}]"
                baseColor="#69C8D5"
                :scale-interval="0"
              />
            </p>
            <div class="visitor_count">
              <div class="returningbox"></div>
              <span>Returning Visitors</span>
              <h2>
                36%
                <small>680</small>
              </h2>
            </div>

            <div class="first_time">
              <div class="returningbox"></div>
              <span>First Time Visitors</span>
              <h2>
                64%
                <small>1240</small>
              </h2>
            </div>
          </div>
          <div class="box_bgcolor mt-5 p-3">
            <p class="box_title">Average posts read or skimmed by visitors before completing a CTA</p>
            <div class="d-flex">
              <div class="w-100 border-right">
                <p>Low:</p>
                <h3 class="font-weight-bold">1</h3>
              </div>
              <div class="w-100">
                <p>High:</p>
                <h3 class="font-weight-bold">19</h3>
              </div>
            </div>
          </div>
          <div>
            <div class="mt-5 p-3 box_bgcolor table-responsive">
              <p class="box_title">Top posts that led to return visits</p>
              <table class="table sample">
                <tbody>
                  <tr class="row">
                    <td class="col-7">sample Title</td>
                    <td class="col-3 text-c2">%95</td>
                    <td class="col-2 op2">
                      <span>
                        <svg
                          aria-hidden="true"
                          focusable="false"
                          data-prefix="fas"
                          data-icon="external-link-alt"
                          role="img"
                          xmlns="http://www.w3.org/2000/svg"
                          viewBox="0 0 512 512"
                          class="svg-inline--fa fa-external-link-alt fa-w-16 fa-3x"
                        >
                          <path
                            fill="currentColor"
                            d="M432,320H400a16,16,0,0,0-16,16V448H64V128H208a16,16,0,0,0,16-16V80a16,16,0,0,0-16-16H48A48,48,0,0,0,0,112V464a48,48,0,0,0,48,48H400a48,48,0,0,0,48-48V336A16,16,0,0,0,432,320ZM488,0h-128c-21.37,0-32.05,25.91-17,41l35.73,35.73L135,320.37a24,24,0,0,0,0,34L157.67,377a24,24,0,0,0,34,0L435.28,133.32,471,169c15,15,41,4.5,41-17V24A24,24,0,0,0,488,0Z"
                            class
                          />
                        </svg>
                      </span>
                    </td>
                  </tr>
                  <tr class="row">
                    <td class="col-7">sample Title</td>
                    <td class="col-3 text-c2">%85</td>
                    <td class="col-2 op2">
                      <span>
                        <svg
                          aria-hidden="true"
                          focusable="false"
                          data-prefix="fas"
                          data-icon="external-link-alt"
                          role="img"
                          xmlns="http://www.w3.org/2000/svg"
                          viewBox="0 0 512 512"
                          class="svg-inline--fa fa-external-link-alt fa-w-16 fa-3x"
                        >
                          <path
                            fill="currentColor"
                            d="M432,320H400a16,16,0,0,0-16,16V448H64V128H208a16,16,0,0,0,16-16V80a16,16,0,0,0-16-16H48A48,48,0,0,0,0,112V464a48,48,0,0,0,48,48H400a48,48,0,0,0,48-48V336A16,16,0,0,0,432,320ZM488,0h-128c-21.37,0-32.05,25.91-17,41l35.73,35.73L135,320.37a24,24,0,0,0,0,34L157.67,377a24,24,0,0,0,34,0L435.28,133.32,471,169c15,15,41,4.5,41-17V24A24,24,0,0,0,488,0Z"
                            class
                          />
                        </svg>
                      </span>
                    </td>
                  </tr>
                  <tr class="row">
                    <td class="col-7">sample Title</td>
                    <td class="col-3 text-c2">%80</td>
                    <td class="col-2 op2">
                      <span>
                        <svg
                          aria-hidden="true"
                          focusable="false"
                          data-prefix="fas"
                          data-icon="external-link-alt"
                          role="img"
                          xmlns="http://www.w3.org/2000/svg"
                          viewBox="0 0 512 512"
                          class="svg-inline--fa fa-external-link-alt fa-w-16 fa-3x"
                        >
                          <path
                            fill="currentColor"
                            d="M432,320H400a16,16,0,0,0-16,16V448H64V128H208a16,16,0,0,0,16-16V80a16,16,0,0,0-16-16H48A48,48,0,0,0,0,112V464a48,48,0,0,0,48,48H400a48,48,0,0,0,48-48V336A16,16,0,0,0,432,320ZM488,0h-128c-21.37,0-32.05,25.91-17,41l35.73,35.73L135,320.37a24,24,0,0,0,0,34L157.67,377a24,24,0,0,0,34,0L435.28,133.32,471,169c15,15,41,4.5,41-17V24A24,24,0,0,0,488,0Z"
                            class
                          />
                        </svg>
                      </span>
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>
        </div>
        <div class="col-md-8 col-sm-12">
          <div>
            <fusioncharts
              type="column2d"
              :width="width"
              height="315"
              :dataformat="dataFormat"
              :dataSource="dataSource"
            ></fusioncharts>
          </div>
          <div>
            <div class="d-flex justify-content-between p-2 mt-3">
              <p>Number of posts viewed per visitor</p>
              <p>Average: 20 per visitor</p>
            </div>
            <fusioncharts
              :type="type"
              :width="width"
              :height="height"
              :dataSource="dataSource1"
            ></fusioncharts>
          </div>
          <div>
            <div class="d-flex justify-content-between p-2 mt-3">
              <p>Number of posts viewed per session</p>
              <p>Average: 20 per session</p>
            </div>
            <fusioncharts
              type="mscolumn2d"
              :width="width"
              :height="height"
              :dataSource="dataSource2"
            ></fusioncharts>
          </div>
        </div>
        <div class="col-12 mt-5 table-responsive">
          <table class="table box_bgcolor visitor_table">
            <thead>
              <tr class>
                <th>Visitor ID</th>
                <th>Status</th>
                <th>Location</th>
                <th># of sessions (30 days)</th>
                <th>Total posts viewed</th>
              </tr>
            </thead>
            <tbody>
              <tr class v-for="(i, index) in visitorData" :key="index">
                <td>{{i.id}}</td>
                <td>{{i.status}}</td>
                <td>{{i.location}}</td>
                <td>{{i.session}}</td>
                <td>{{i.post}}</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import VueFusionCharts from "vue-fusioncharts";
import FusionCharts from "fusioncharts";
import Column2D from "fusioncharts/fusioncharts.charts";
import FusionTheme from "fusioncharts/themes/fusioncharts.theme.fusion";
import Vue from "vue";
Vue.use(VueFusionCharts, FusionCharts, Column2D, FusionTheme);

const chartData = [
  {
    label: "NOV 15",
    value: "300"
  },
  {
    label: "NOV 16",
    value: "200"
  },
  {
    label: "NOV 17",
    value: "420"
  },
  {
    label: "NOV 18",
    value: "300"
  },
  {
    label: "NOV 19",
    value: "200"
  },
  {
    label: "NOV 20",
    value: "420"
  },
  {
    label: "NOV 21",
    value: "200"
  }
];

// STEP 3: Configure your chart

export default {
  name: "WrittioDashboard",
  data() {
    return {
      visitorData: [
        {
          id: "Visitor123",
          status: "Logged out",
          location: "US",
          session: 4,
          post: 11
        },
        {
          id: "Visitor123",
          status: "Logged out",
          location: "US",
          session: 4,
          post: 11
        },
        {
          id: "Visitor123",
          status: "Logged out",
          location: "US",
          session: 4,
          post: 11
        }
      ],
      blogVisitor: "29,954",

      type: "mscolumn2d",
      renderAt: "chart-container",
      width: "100%",
      height: "315",
      dataFormat: "json",
      dataSource1: {
        chart: {
          caption: "",
          xAxisname: "",
          yAxisName: "",
          numberPrefix: "",
          numbersuffix: "",
          plotFillAlpha: "80",
          paletteColors: "#7480FF",
          theme: "fusion",
          plotSpacePercent: "0",
          plotPaddingPercent: "20",
          yAxisMaxValue: "25"
        },
        categories: [
          {
            category: [
              {
                label: "NOV 15"
              },
              {
                label: "NOV 16"
              },
              {
                label: "NOV 17"
              },
              {
                label: "NOV 18"
              },
              {
                label: "NOV 19"
              },
              {
                label: "NOV 20"
              },
              {
                label: "NOV 21"
              }
            ]
          }
        ],
        dataset: [
          {
            data: [
              {
                value: "15"
              },
              {
                value: "15"
              },
              {
                value: "10"
              },
              {
                value: "24"
              },
              {
                value: "24"
              },
              {
                value: "18"
              },
              {
                value: "18"
              }
            ]
          },
          {
            data: [
              {
                value: "10"
              },
              {
                value: "10"
              },
              {
                value: "15"
              },
              {
                value: "15"
              },
              {
                value: "18"
              },
              {
                value: "24"
              },
              {
                value: "15"
              }
            ]
          },
          {
            data: [
              {
                value: "24"
              },
              {
                value: "24"
              },
              {
                value: "10"
              },
              {
                value: "18"
              },
              {
                value: "15"
              },
              {
                value: "18"
              },
              {
                value: "24"
              }
            ]
          }
        ]
      },
      dataSource2: {
        chart: {
          caption: "",
          xAxisname: "",
          yAxisName: "",
          numberPrefix: "",
          plotFillAlpha: "80",
          paletteColors: "#69C9D6",
          theme: "fusion",
          plotSpacePercent: "0",
          plotPaddingPercent: "20",
          yAxisMaxValue: "25"
        },
        categories: [
          {
            category: [
              {
                label: "NOV 15"
              },
              {
                label: "NOV 16"
              },
              {
                label: "NOV 17"
              },
              {
                label: "NOV 18"
              },
              {
                label: "NOV 19"
              },
              {
                label: "NOV 20"
              },
              {
                label: "NOV 21"
              }
            ]
          }
        ],
        dataset: [
          {
            data: [
              {
                value: "15"
              },
              {
                value: "15"
              },
              {
                value: "10"
              },
              {
                value: "24"
              },
              {
                value: "24"
              },
              {
                value: "18"
              },
              {
                value: "18"
              }
            ]
          },
          {
            data: [
              {
                value: "10"
              },
              {
                value: "10"
              },
              {
                value: "15"
              },
              {
                value: "15"
              },
              {
                value: "18"
              },
              {
                value: "24"
              },
              {
                value: "15"
              }
            ]
          },
          {
            data: [
              {
                value: "24"
              },
              {
                value: "24"
              },
              {
                value: "10"
              },
              {
                value: "18"
              },
              {
                value: "15"
              },
              {
                value: "18"
              },
              {
                value: "24"
              }
            ]
          }
        ]
      },
      dataSource: {
        chart: {
          caption: "",
          subcaption: "",
          xaxisname: "",
          yaxisname: "",
          numbersuffix: "",
          paletteColors: "#FDD32A",
          theme: "fusion",
          plotSpacePercent: "60"
        },
        data: chartData
      }
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import "../assets/style.css";
</style>
