<template>
  <div class="relative">
    <ScheduleHeader day="06" />
    <ScheduleEventSimple
      start="07:30" end="08:00"
      title="Credênciamento | Minicursos"
    />
    <!-- Courses line display for large screens -->
    <div class="hidden flex-row md:flex md:gap-2">
      <ScheduleEventCourse
        start="08:00" end="10:00"
        title="EM BREVE MAIS INFORMAÇÕES"
        extra="Minicurso"
        speaker="Fique ligado!"
        position="Nos siga no instragram para ficar por dentro das novidades @encompceunes"
      />
      <ScheduleEventCourse
        start="08:00" end="10:00"
        title="EM BREVE MAIS INFORMAÇÕES"
        extra="Minicurso"
        speaker="Fique ligado!"
        position="Nos siga no instragram para ficar por dentro das novidades @encompceunes"
      />
    </div>
    <!-- Courses line carousel display for small screens -->
    <div class="lg:hidden">
      <Carousel>
        <CarouselContent>
          <CarouselItem>
            <ScheduleEventCourse
              start="08:00" end="10:00"
              title="EM BREVE MAIS INFORMAÇÕES"
              extra="Minicurso"
              speaker="Fique ligado!"
              position="Nos siga no instragram para ficar por dentro das novidades @encompceunes"
              :show-arrow="true"
            />
          </CarouselItem>
          <CarouselItem>
            <ScheduleEventCourse
              start="08:00" end="10:00"
              title="EM BREVE MAIS INFORMAÇÕES"
              extra="Minicurso"
              speaker="Fique ligado!"
              position="Nos siga no instragram para ficar por dentro das novidades @encompceunes"
            />
          </CarouselItem>
        </CarouselContent>
      </Carousel>
    </div>
    <ScheduleBreak start="10:00" end="10:30" class="my-3" title="Coffee Break" />
    <!-- Courses line display for large screens -->
    <div class="hidden flex-row md:flex md:gap-2">
      <ScheduleEventCourse
        start="10:30" end="12:00"
        title="EM BREVE MAIS INFORMAÇÕES"
        extra="Minicurso"
        speaker="Fique ligado!"
        position="Nos siga no instragram para ficar por dentro das novidades @encompceunes"
      />
      <ScheduleEventCourse
        start="10:30" end="12:00"
        title="EM BREVE MAIS INFORMAÇÕES"
        extra="Minicurso"
        speaker="Fique ligado!"
        position="Nos siga no instragram para ficar por dentro das novidades @encompceunes"
      />
    </div>
    <!-- Courses line carousel display for small screens -->
    <div class="lg:hidden">
      <Carousel>
        <CarouselContent>
          <CarouselItem>
            <ScheduleEventCourse
              start="10:30" end="12:00"
              title="EM BREVE MAIS INFORMAÇÕES"
              extra="Minicurso"
              speaker="Fique ligado!"
              position="Nos siga no instragram para ficar por dentro das novidades @encompceunes"
              :show-arrow="true"
            />
          </CarouselItem>
          <CarouselItem>
            <ScheduleEventCourse
              start="10:00" end="12:00"
              title="EM BREVE MAIS INFORMAÇÕES"
              extra="Minicurso"
              speaker="Fique ligado!"
              position="Nos siga no instragram para ficar por dentro das novidades @encompceunes"
            />
          </CarouselItem>
        </CarouselContent>
      </Carousel>
    </div>
    <ScheduleBreak start="12:00" end="12:30" class="my-3" title="Intervalo para Almoço" />
    <ScheduleEventSimple
      start="12:30" end="13:00"
      title="Credênciamento | Palestras"
      extra="Auditório"
    />
    <ScheduleEventSimple start="13:00" end="13:15" title="Abertura" />
    <ScheduleEventTalk
      start="13:15" end="14:05"
      title="Dos Blogs à Engenharia de Software: Como Transformei Minha Carreira na Técnologia"
      speaker="Beatriz Duarte"
      description="Vou contar um pouco sobre minha trajetória até me tornar Engenheira de Software, erros e acertos que cometi ao longo desses mais de 10 anos desde que escrevi minhas primeiras linhas de código, além de conselhos para quem quiser seguir na área de desenvolvimento de software"
      :show-description="true"
      position="Engenheira de Software no Nubank"
      photo="/speakers/beatriz_duarte.png"
    />
    <ScheduleEventSimple start="14:05" end="14:25" title="Momento Alura" color="text-blue-500" />
    <ScheduleEventTalk
      start="14:30" end="16:30"
      title="Mesa Redonda: Bate Papo com Professores"
      speaker="Professores do Departamento de Computação e Eletrônica"
      description="Um bate papo com professores dos cursos de Ciência e Engenharia da Computação, com trocas de experiências e a abertura de um momento ideal para quem pretende cursar o ensino superior na UFES tirar dúvidas e conhecer mais do ambiente acadêmico"
      photo=""
    />
    <ScheduleEventTalk
      start="16:40" end="17:30"
      title="Como se Tornar Indispensável na Era da Inteligência Artificial"
      speaker="Patrick Bonometti"
      description="Iremos explorar o impacto transformador da Inteligência Artificial no mercado de trabalho contemporâneo. Discutiremos como essa nova era está redefinindo funções e habilidades, e como você pode se adaptar e prosperar nesse ambiente em constante mudança"
      :show-description="true"
      position="Fundador da IA Valley"
      photo="/speakers/patrick_bonometti.png"
    />
  </div>
  <ScheduleEventSimple start="17:30" end="17:40" title="Avisos e Sorteios" />
  <ScheduleBreak start="17:40" end="18:00" title="Coffee Break | Encerramento" />
  <div class="my-32 min-h-20" />
</template>
