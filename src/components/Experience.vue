<template>
    <v-row v-for="experience in experiences"
            :key="experience.company">
        <v-col
            align-self="center">
            <v-card align-center align-self="center">
                <v-card-title class="d-flex align-center">
                    {{ experience.company }}
                </v-card-title>
                <v-card-text>
                    <p class="font-weight-black">
                        {{ experience.title }}
                    </p>
                    <p class="font-italic">
                        {{ 'Location: ' + experience.location }}
                        <br/>
                        {{ 'Duration: ' + experience.startDate + ' - ' + experience.endDate }}
                    </p>
                    <p class="font-weight-light" v-for="detail in experience.info">
                        {{ '- ' + detail }}
                    </p>
                </v-card-text>
            </v-card>
        </v-col>
    </v-row>
</template>

<script>
export default {
    data() {
        return {
            experiences: [
            {
                    company: 'ECIJA',
                    title: 'Legal Intern',
                    location: 'Madrid, Spain',
                    startDate: 'June 2024',
                    endDate: 'Present',
                    info: [
                        'IP/IT Department - ECIJA being a pioneer firm in the Technology, Media and Telecommunications sector, as well as  leader in TMT advice to companies in Spain.',
                        'Part of the "Programa de Prácticas #EcijaChallenge", in order to receive an insight on the law firm, its work and take part in their day-to-day operations.'
                    ]
                },
                {
                    company: 'Meraki Smile School',
                    title: 'Lead Marketing and Social Media Manager',
                    location: 'Madagascar (Remote)',
                    startDate: 'February 2022',
                    endDate: 'Present',
                    info: [
                        'Seeking and investigating new potential partnerships at both local and international levels.',
                        'Drafting and designing partnership proposals, communicating the mission of the organization and its alignment with diverse institutions` values.',
                        'Establishing collaborations with institutions, fostering mutual growth and securing vital resources and opportunities for our students.',
                        'Participating in the initial stages of implementing new synergies between Meraki Smile School and partner institutions.',
                        'Coordinated the content and marketing strategy, and the team.',
                        'Content creation for various platforms, and managed social media to increase awareness, engagement and knowledge of the organization.'
                    ]
                },
                {
                    company: 'IE University Legal Clinic',
                    title: 'Pro Bono Legal Consultant and Teaching Assistant',
                    location: 'Madrid, Spain',
                    startDate: 'January 2024',
                    endDate: 'June 2024',
                    info: [
                        'As a Senior Student, I oversaw team coordination, managed work distribution, and facilitated both internal and external communications. Additionally, respond to inquiries from peers and ensure efficient project execution.',
                        'My research was focused on Corporate Legislation and Governance applied to non-profit organizations, more specifically on measures to increase diversity in the board of directs and democratization of decision-making.',
                        ' The legal research included state, federal and comparative law, in order to draft the recommendations from a holistic approach.',
                        'The objective is to provide a guide comprising regulations, interpretations and recommendations surrounding the democratization and diversity of non-profit organizations in Massachusetts/New England.'
                    ]
                },
                {
                    company: 'IE University',
                    title: 'Research Assistant',
                    location: 'Madrid, Spain',
                    startDate: 'January 2024',
                    endDate: 'Present',
                    info: [
                        'Assisting the formulation and implementation of the investigation of Carlos Lastra and Elsa Voytas, surrounding the impact of art in political, historical and interpersonal perceptions of young people.'
                    ]
                },
                {
                    company: 'Delyser Abogados',
                    title: 'Legal Intern',
                    location: 'Madrid, Spain',
                    startDate: 'January 2024',
                    endDate: 'April 2024',
                    info: [
                        'Rotating and assisting in the different legislative specialities.',
                        'Providing support for the different specializations of the firm.',
                        'Research & Investigation',
                        'Drafting of legal documents'
                    ]
                },
                {
                    company: 'Arts & Business Council of Greater Boston',
                    title: 'Legal Intern',
                    location: 'Boston, United States',
                    startDate: 'September 2023',
                    endDate: 'December 2023',
                    info: [
                        'Took part in the Volunteer Lawyers for the Arts (VLA) Team.',
                        'Conducted legal research, prepared written legal analyses, and attended client counselling sessions.',
                        'Reviewed and recorded legal services applications.',
                        'Assisted with other matters appropriate for a Legal Intern as they arose.'
                    ]
                },
                {
                    company: 'Luxury WVS Real Estate',
                    title: 'Public Relations and Social Media Manager',
                    location: 'La Romana, Dominican Republic (Remote)',
                    startDate: 'January 2023',
                    endDate: 'July 2023',
                    info: [
                        'Developed and Implemented Marketing Strategies: increased the visibility of the brand.',
                        'Social Media and Brand Management: Successfully enhanced the social media presence of the brand.',
                        'Content Creation and Curation: Produced engaging and shareable content.',
                        'Data Analysis and Insights: Utilized analytics tools to measure performance and gather insights for continuous improvement.',
                        'Establishing and developing collaboration opportunities with local businesses.'
                    ]
                },
                {
                    company: 'IE University Legal Clinic',
                    title: 'Pro Bono Legal Consultant',
                    location: 'Madrid, Spain',
                    startDate: 'January 2023',
                    endDate: 'May 2023',
                    info: [
                        'Carried out consultancy on child protection in Madagascar for the NGO Meraki Smile School.',
                        'Legal research on local, international and comparative law, in order to draft the recommendations from a holistic approach.',
                        'We drafted a guide comprising regulations, interpretations and recommendations.',
                        'We also considered the the translation of this guide into different formats in order to transmit its contents in a more effective and personalized manner to different stakeholders (students, volunteers and staff).'
                    ]
                },
                {
                    company: 'EFE Europe',
                    title: 'Business Development and Communications Intern',
                    location: 'Madrid, Spain',
                    startDate: 'March 2023',
                    endDate: 'May 2023',
                    info: [
                        'Assisted in the development of the development and implementation of marketing strategies, as well as in social media and brand management. Considering the network of organizations EFE comprises, collaboration with cross-organizational teams was vital.',
                        'Provided valuable support in various aspects of business development, ranging from conducting research tasks to crafting compelling content.',
                        'Gained insights into the intricate internal mechanisms of the organization, emphasizing the significance of effective communication and reporting within the management structure.',
                    ]
                },
                {
                    company: 'OH! Tours',
                    title: 'Tour Guide',
                    location: 'Porto, Portugal',
                    startDate: 'July 2022',
                    endDate: 'August 2022',
                    info: [
                        'Conducted extensive research and acquiring profound insights into the historical and artistic heritage of Porto, to provide enriching experiences for clients.',
                        'Delivered attentive and knowledgeable customer service as a dedicated guide, leading clients on captivating tours through various points of interest in the city.'
                    ]
                },
                {
                    company: 'IE University Policy Lab',
                    title: 'Internal Coordinator',
                    location: 'Madrid, Spain',
                    startDate: 'February 2021',
                    endDate: 'June 2021',
                    info: [
                        'Collaborated with UNICEF Egypt to provide a situation analysis and background research on refugees in Egypt.',
                        'The objective of our research was the available or potential help to children in terms of housing, education and healthcare.',
                        'My responsibilities within the team, alongside the inherent work of research and drafting of the proposal, was internal coordination, in order to ensure the organization and efficiency of the team.'
                    ]
                },
            ]
        }
    }
}
</script>