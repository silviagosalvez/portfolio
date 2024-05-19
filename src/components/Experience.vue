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
                        'Selected to assist in the IP/IT Department for Technology, Media, Telecommunications, and other sectors '
                        + 'as a part of the Programa de Prácticas #EcijaChallenge in order to receive an insight on the law firm'
                        + " its work and take part in their day-to-day operations."
                    ]
                },
                {
                    company: 'Meraki Smile School',
                    title: 'Lead Marketing and Social Media Manager',
                    location: 'Madagascar (Remote)',
                    startDate: 'February 2022',
                    endDate: 'Present',
                    info: [
                        'Investigated new potential partnerships at both local and international levels.',
                        'Designed partnership proposals to communicate the mission of the organization and its alignment '
                        + "with other institutions' values.",
                        'Collaborated with institutions, fostering mutual growth while securing vital resources and' 
                        + ' opportunities for our students.',
                        'Participated in the initial stages of implementing new synergies between Meraki Smile School '
                        + 'and partner institutions.',
                        'Coordinated the marketing strategy and created content for various platforms to increase '
                        + 'awareness, engagement and knowledge of the organization.',
                    ]
                },
                {
                    company: 'IE University Legal Clinic',
                    title: 'Pro Bono Legal Consultant and Teaching Assistant',
                    location: 'Madrid, Spain',
                    startDate: 'January 2024',
                    endDate: 'June 2024',
                    info: [
                        'Oversaw team coordination, managed work distribution, and facilitated both internal and external '
                        + 'communications.',
                        'Responded to inquiries from peers and ensure efficient project execution.',
                        'Researched Corporate Legislation and Governance as can be applied to non-profit organizations, '
                        + 'to increase diversity in the board of directors and democratize decision-making.',
                        'Coordinated the communications of the lab with both directors, studnets, and other IE departments.',
                    ]
                },
                {
                    company: 'IE University',
                    title: 'Research Assistant',
                    location: 'Madrid, Spain',
                    startDate: 'January 2024',
                    endDate: 'Present',
                    info: [
                        'Assisted in the formulation and implementation of the investigation of Carlos Lastra and Elsa Voytas, '
                        + 'surrounding the impact of art in political, historical and interpersonal perceptions of young people.'
                    ]
                },
                {
                    company: 'Delyser Abogados',
                    title: 'Legal Intern',
                    location: 'Madrid, Spain',
                    startDate: 'January 2024',
                    endDate: 'April 2024',
                    info: [
                        'Assisted in the different legislative specialities of the firm, primarity in commercial law matters '
                        + 'by researching and investigating information for drafting and translating of legal documents.'
                    ]
                },
                {
                    company: 'Arts & Business Council of Greater Boston',
                    title: 'Legal Intern in the Volunteer Lawyers for the Arts (VLA) Team',
                    location: 'Boston, United States',
                    startDate: 'September 2023',
                    endDate: 'December 2023',
                    info: [
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
                        'Developed and Implemented Marketing Strategies which increased the visibility of the brand.',
                        'Increase the social media presence of the Luxury WVS Real Estate brand by 950%.',
                        "Produced and curated engaging and shareable content for the Luxury WVS Real Estate's social media account.",
                        'Utilized analytic tools to measure performance and gather insights for continuous improvement.',
                        'Established and developed collaborative opportunities with other local businesses.'
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
                        'Researched local, international and comparative law, in order to make recommendations '
                        + 'from a more holistic approach.',
                        'Established a comprehensive guide comprising regulations, interpretations and recommendations '
                        + "for the client's use.",
                    ]
                },
                {
                    company: 'EFE Europe',
                    title: 'Business Development and Communications Intern',
                    location: 'Madrid, Spain',
                    startDate: 'March 2023',
                    endDate: 'May 2023',
                    info: [
                        'Assisted in the development and implementation of new marketing strategies.',
                        "Aided in the management of both branding and the companies' social media account",
                        'Collaborated with the cross-organizational that the network of organizations EFE comprises.',
                        'Supported business development by conducting research tasks and crafting compelling content.',
                    ]
                },
                {
                    company: 'OH! Tours',
                    title: 'Tour Guide',
                    location: 'Porto, Portugal',
                    startDate: 'July 2022',
                    endDate: 'August 2022',
                    info: [
                        'Conducted extensive research and acquired profound insights into the historical and artistic'
                        + ' heritage of Porto to provide enriching experiences for clients.',
                        'Delivered attentive and knowledgeable customer service as a dedicated guide, leading clients'
                        +' on captivating tours through various points of interest in the city.'
                    ]
                },
            ]
        }
    }
}
</script>