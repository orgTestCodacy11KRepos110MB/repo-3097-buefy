<template>
    <div>
        <Example :component="ExSimple" :code="ExSimpleCode" vertical/>

        <Example :component="ExDragDrop" :code="ExDragDropCode" title="Drag and drop" vertical/>
        
        <Example :component="ExExpanded" :code="ExExpandedCode" title="Expanded" vertical/>
        
        <Example :component="ExRounded" :code="ExRoundedCode" title="Rounded" vertical/>
        
        <Example :component="ExValidation" :code="ExValidationCode" title="Validation" vertical/>

        <ApiView :data="api"/>
    </div>
</template>

<script>
    import api from './api/upload'

    import ExSimple from './examples/ExSimple'
    import ExSimpleCode from '!!raw-loader!./examples/ExSimple'

    import ExDragDrop from './examples/ExDragDrop'
    import ExDragDropCode from '!!raw-loader!./examples/ExDragDrop'

    import ExExpanded from './examples/ExExpanded'
    import ExExpandedCode from '!!raw-loader!./examples/ExExpanded'    
    
    import ExRounded from './examples/ExRounded'
    import ExRoundedCode from '!!raw-loader!./examples/ExRounded'

    import ExValidation from './examples/ExValidation'
    import ExValidationCode from '!!raw-loader!./examples/ExValidation'


    export default {
        data() {
            return {
                api,
                ExSimple,
                ExDragDrop,
                ExExpanded,
                ExSimpleCode,
                ExDragDropCode,
                ExExpandedCode,
                ExRounded,
                ExRoundedCode,
                ExValidation,
                ExValidationCode,
            }
        }
    }
</script>
