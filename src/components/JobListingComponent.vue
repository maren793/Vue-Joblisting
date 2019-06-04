 <template>
        <div class="[ card ]">
            <div class="row">
                <div class="[ col-sm-4 ]"></div>
                <div class="[ col-sm-4 ]"><img :src="jobImg" /><br /><br /><br /></div>
                <div class="[ col-sm-4 ]"></div>
                </div>
                <div class="[ card--information ]"><br />
                    <b>Date Created: </b>{{dateCreated}} <br />
                    <b>Title: </b> {{title}} <br />
                    <b>company Name: </b> {{companyName}} <br />
                    <b>Location: </b> {{location}} <br />
                    <b>Type: </b> {{type}} <br />
                    <b>Description: </b><span v-html="description"></span><br />
                    <b>How to apply: </b> <span v-html="HowToApply"></span><br />
                    <b>Company Website: </b><a :href="website" target="_blank">Click here</a> <br />
                </div>
            </div>
</template>

<script>
export default {
    name: 'JobListingComponent',
    props: ['jobImg', 'dateCreated', 'title', 'companyName', 'location', 'type', 'description', 'howToApply', 'website'],
}
</script>