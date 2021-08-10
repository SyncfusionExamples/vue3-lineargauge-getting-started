<template>
    <ejs-lineargauge :title ='title' orientation='Horizontal'>
        <e-axes>
            <e-axis minimum=0 maximum=200>
                <e-pointers>
                    <e-pointer value=140 color='red'></e-pointer>
                </e-pointers>
                <e-ranges>
                    <e-range start=0 end=80 startWidth=15 endWidth=15></e-range>
                    <e-range start=80 end=120 startWidth=15 endWidth=15></e-range>
                    <e-range start=120 end=140 startWidth=15 endWidth=15></e-range>
                    <e-range start=140 end=200 startWidth=15 endWidth=15></e-range>
                </e-ranges>
            </e-axis>
        </e-axes>
    </ejs-lineargauge>
</template>

<script>
import { LinearGaugeComponent, AxesDirective, AxisDirective, PointersDirective, PointerDirective, RangesDirective, RangeDirective } from '@syncfusion/ej2-vue-lineargauge'

export default {
  name: 'App',
  components: {
    'ejs-lineargauge' : LinearGaugeComponent,
    'e-axes' : AxesDirective,
    'e-axis' : AxisDirective,
    'e-pointers': PointersDirective,
    'e-pointer' : PointerDirective,
    'e-ranges' : RangesDirective,
    'e-range' : RangeDirective
  },
  data: function () {
      return {
          title: 'Linear Gauge',
      }
  }
}
</script>
