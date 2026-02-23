Слайдер с крупными стрелками (фиксированный размер)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: html+django

   <div class="row justify-content-center">
       <div class="col-12">
           <div id="courseSliderLarge" class="carousel slide" data-bs-ride="carousel">
               <div class="carousel-indicators">
                   <button type="button" data-bs-target="#courseSliderLarge" data-bs-slide-to="0" class="active"></button>
                   <button type="button" data-bs-target="#courseSliderLarge" data-bs-slide-to="1"></button>
                   <button type="button" data-bs-target="#courseSliderLarge" data-bs-slide-to="2"></button>
                   <button type="button" data-bs-target="#courseSliderLarge" data-bs-slide-to="3"></button>
               </div>
               
               <div class="carousel-inner rounded-4" style="height: 500px;">
                   {# Слайд 1 - Программирование #}
                   <div class="carousel-item active h-100">
                       <img src="{% static 'images/slide1.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Курсы программирования">
                       <div class="carousel-caption d-none d-md-block p-4 bg-dark bg-opacity-50 rounded">
                           <h4 class="fw-bold">Основы программирования</h4>
                           <p class="fs-5">Научитесь основам программирования и созданию алгоритмов</p>
                       </div>
                   </div>
                   
                   {# Слайд 2 - Веб-дизайн #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide2.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Веб-дизайн">
                       <div class="carousel-caption d-none d-md-block p-4 bg-dark bg-opacity-50 rounded">
                           <h4 class="fw-bold">Основы веб-дизайна</h4>
                           <p class="fs-5">Освойте современные тенденции в создании веб-интерфейсов</p>
                       </div>
                   </div>
                   
                   {# Слайд 3 - Базы данных #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide3.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Базы данных">
                       <div class="carousel-caption d-none d-md-block p-4 bg-dark bg-opacity-50 rounded">
                           <h4 class="fw-bold">Проектирование баз данных</h4>
                           <p class="fs-5">Изучите принципы проектирования и работы с базами данных</p>
                       </div>
                   </div>
                   
                   {# Слайд 4 - Документы #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide4.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Дипломы">
                       <div class="carousel-caption d-none d-md-block p-4 bg-dark bg-opacity-50 rounded">
                           <h4 class="fw-bold">Официальные документы</h4>
                           <p class="fs-5">Получите документы об образовании после завершения курсов</p>
                       </div>
                   </div>
               </div>
               
               <button class="carousel-control-prev" type="button" data-bs-target="#courseSliderLarge" data-bs-slide="prev">
                   <span class="carousel-control-prev-icon" style="width: 60px; height: 60px;" aria-hidden="true"></span>
                   <span class="visually-hidden">Предыдущий</span>
               </button>
               <button class="carousel-control-next" type="button" data-bs-target="#courseSliderLarge" data-bs-slide="next">
                   <span class="carousel-control-next-icon" style="width: 60px; height: 60px;" aria-hidden="true"></span>
                   <span class="visually-hidden">Следующий</span>
               </button>
           </div>
       </div>
   </div>

**Описание:** Первый вариант слайдера с крупными стрелками навигации (60×60 пикселей) и фиксированной высотой контейнера (500px). Используется для главных промо-материалов на странице.

Слайдер с текстовыми стрелками (фиксированный размер)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: html+django

   {# Компактный слайдер с текстовыми стрелками #}
   <div class="row justify-content-center">
       <div class="col-12 col-lg-8">
           <div id="courseSliderCompact" class="carousel slide" data-bs-ride="carousel">
               <div class="carousel-inner rounded shadow-sm" style="height: 300px;">
                   {# Слайд 1 - Программирование #}
                   <div class="carousel-item active h-100">
                       <img src="{% static 'images/slide1.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Курсы программирования">
                       <div class="carousel-caption text-start p-3">
                           <h6 class="mb-1">Основы алгоритмизации</h6>
                           <p class="small mb-2">Научитесь основам программирования</p>
                       </div>
                   </div>
                   
                   {# Слайд 2 - Веб-дизайн #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide2.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Веб-дизайн">
                       <div class="carousel-caption text-start p-3">
                           <h6 class="mb-1">Веб-дизайн</h6>
                           <p class="small mb-2">Современные интерфейсы и UX/UI</p>
                       </div>
                   </div>
                   
                   {# Слайд 3 - Базы данных #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide3.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Базы данных">
                       <div class="carousel-caption text-start p-3">
                           <h6 class="mb-1">Базы данных</h6>
                           <p class="small mb-2">Проектирование и SQL</p>
                       </div>
                   </div>
                   
                   {# Слайд 4 - Документы #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide4.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Дипломы">
                       <div class="carousel-caption text-start p-3">
                           <h6 class="mb-1">Документы</h6>
                           <p class="small mb-2">Официальное подтверждение навыков</p>
                       </div>
                   </div>
               </div>
               
               <div class="carousel-indicators position-static mt-3 justify-content-center">
                   <button type="button" data-bs-target="#courseSliderCompact" data-bs-slide-to="0" class="active mx-1"></button>
                   <button type="button" data-bs-target="#courseSliderCompact" data-bs-slide-to="1" class="mx-1"></button>
                   <button type="button" data-bs-target="#courseSliderCompact" data-bs-slide-to="2" class="mx-1"></button>
                   <button type="button" data-bs-target="#courseSliderCompact" data-bs-slide-to="3" class="mx-1"></button>
               </div>
               
               <button class="carousel-control-prev" type="button" data-bs-target="#courseSliderCompact" data-bs-slide="prev" style="width: 40px; background: rgba(0,0,0,0.2);">
                   <span style="font-size: 2rem; color: white; font-weight: bold;">‹</span>
                   <span class="visually-hidden">Предыдущий</span>
               </button>
               <button class="carousel-control-next" type="button" data-bs-target="#courseSliderCompact" data-bs-slide="next" style="width: 40px; background: rgba(0,0,0,0.2);">
                   <span style="font-size: 2rem; color: white; font-weight: bold;">›</span>
                   <span class="visually-hidden">Следующий</span>
               </button>
           </div>
       </div>
   </div>

**Описание:** Второй вариант слайдера с текстовыми стрелками навигации (символы ‹ и ›) и компактным дизайном. Индикаторы расположены под слайдером, высота контейнера - 300px. Используется для второстепенных промо-блоков.

Слайдер с круглыми стрелками (фиксированный размер)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: html+django

   {# Слайдер с плавающими стрелками #}
   <div class="row justify-content-center">
       <div class="col-12 col-xl-9">
           <div id="courseSliderFloating" class="carousel slide" data-bs-ride="carousel">
               <div class="carousel-inner rounded-3 overflow-hidden shadow" style="height: 450px;">
                   {# Слайд 1 - Программирование #}
                   <div class="carousel-item active h-100">
                       <img src="{% static 'images/slide1.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Курсы программирования">
                       <div class="carousel-caption d-none d-md-block bg-gradient rounded-bottom p-4">
                           <h5 class="text-white">Основы программирования</h5>
                           <p class="text-light">Изучите базовые концепции и алгоритмы</p>
                       </div>
                   </div>
                   
                   {# Слайд 2 - Веб-дизайн #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide2.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Веб-дизайн">
                       <div class="carousel-caption d-none d-md-block bg-gradient rounded-bottom p-4">
                           <h5 class="text-white">Веб-дизайн</h5>
                           <p class="text-light">Создавайте современные интерфейсы</p>
                       </div>
                   </div>
                   
                   {# Слайд 3 - Базы данных #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide3.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Базы данных">
                       <div class="carousel-caption d-none d-md-block bg-gradient rounded-bottom p-4">
                           <h5 class="text-white">Базы данных</h5>
                           <p class="text-light">Проектируйте и оптимизируйте данные</p>
                       </div>
                   </div>
                   
                   {# Слайд 4 - Документы #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide4.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Дипломы">
                       <div class="carousel-caption d-none d-md-block bg-gradient rounded-bottom p-4">
                           <h5 class="text-white">Сертификация</h5>
                           <p class="text-light">Получите подтверждение ваших навыков</p>
                       </div>
                   </div>
               </div>
               
               <button class="carousel-control-prev" type="button" data-bs-target="#courseSliderFloating" data-bs-slide="prev" style="width: 50px; opacity: 0.8;">
                   <span style="background: white; border-radius: 50%; width: 40px; height: 40px; display: flex; align-items: center; justify-content: center; color: #333; font-weight: bold; box-shadow: 0 2px 5px rgba(0,0,0,0.3);">❮</span>
                   <span class="visually-hidden">Предыдущий</span>
               </button>
               <button class="carousel-control-next" type="button" data-bs-target="#courseSliderFloating" data-bs-slide="next" style="width: 50px; opacity: 0.8;">
                   <span style="background: white; border-radius: 50%; width: 40px; height: 40px; display: flex; align-items: center; justify-content: center; color: #333; font-weight: bold; box-shadow: 0 2px 5px rgba(0,0,0,0.3);">❯</span>
                   <span class="visually-hidden">Следующий</span>
               </button>
               
               <div class="carousel-indicators" style="bottom: 20px;">
                   <button type="button" data-bs-target="#courseSliderFloating" data-bs-slide-to="0" class="active"></button>
                   <button type="button" data-bs-target="#courseSliderFloating" data-bs-slide-to="1"></button>
                   <button type="button" data-bs-target="#courseSliderFloating" data-bs-slide-to="2"></button>
                   <button type="button" data-bs-target="#courseSliderFloating" data-bs-slide-to="3"></button>
               </div>
           </div>
       </div>
   </div>

**Описание:** Третий вариант слайдера с круглыми плавающими стрелками навигации. Стрелки имеют белый фон с тенью, расположены поверх изображения. Высота контейнера - 450px. Используется для привлечения внимания к ключевым предложениям.

Минималистичный слайдер (фиксированный размер)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: html+django

   {# Минималистичный слайдер #}
   <div class="row justify-content-center">
       <div class="col-12 col-lg-10">
           <div id="courseSliderMinimal" class="carousel slide" data-bs-ride="carousel" data-bs-interval="4000">
               <div class="carousel-inner" style="height: 400px;">
                   {# Слайд 1 - Программирование #}
                   <div class="carousel-item active h-100">
                       <img src="{% static 'images/slide1.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover; border-radius: 8px;" alt="Курсы программирования">
                       <div class="carousel-caption d-none d-md-block" style="bottom: 30px; left: 30px; right: auto; text-align: left; background: rgba(255,255,255,0.9); padding: 15px; border-radius: 8px; max-width: 400px;">
                           <div>
                               <h5 class="mb-2">Основы алгоритмизации</h5>
                               <p class="mb-0">Старт карьеры в IT</p>
                           </div>
                       </div>
                   </div>
                   
                   {# Слайд 2 - Веб-дизайн #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide2.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover; border-radius: 8px;" alt="Веб-дизайн">
                       <div class="carousel-caption d-none d-md-block" style="bottom: 30px; left: 30px; right: auto; text-align: left; background: rgba(255,255,255,0.9); padding: 15px; border-radius: 8px; max-width: 400px;">
                           <div>
                               <h5 class="mb-2">Веб-дизайн</h5>
                               <p class="mb-0">Создание интерфейсов</p>
                           </div>
                       </div>
                   </div>
                   
                   {# Слайд 3 - Базы данных #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide3.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover; border-radius: 8px;" alt="Базы данных">
                       <div class="carousel-caption d-none d-md-block" style="bottom: 30px; left: 30px; right: auto; text-align: left; background: rgba(255,255,255,0.9); padding: 15px; border-radius: 8px; max-width: 400px;">
                           <div>
                               <h5 class="mb-2">Базы данных</h5>
                               <p class="mb-0">Хранение и управление</p>
                           </div>
                       </div>
                   </div>
                   
                   {# Слайд 4 - Документы #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide4.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover; border-radius: 8px;" alt="Дипломы">
                       <div class="carousel-caption d-none d-md-block" style="bottom: 30px; left: 30px; right: auto; text-align: left; background: rgba(255,255,255,0.9); padding: 15px; border-radius: 8px; max-width: 400px;">
                           <div>
                               <h5 class="mb-2">Сертификация</h5>
                               <p class="mb-0">Официальное подтверждение</p>
                           </div>
                       </div>
                   </div>
               </div>
               
               <div class="carousel-indicators">
                   <button type="button" data-bs-target="#courseSliderMinimal" data-bs-slide-to="0" class="active" style="width: 8px; height: 8px; border-radius: 50%;"></button>
                   <button type="button" data-bs-target="#courseSliderMinimal" data-bs-slide-to="1" style="width: 8px; height: 8px; border-radius: 50%;"></button>
                   <button type="button" data-bs-target="#courseSliderMinimal" data-bs-slide-to="2" style="width: 8px; height: 8px; border-radius: 50%;"></button>
                   <button type="button" data-bs-target="#courseSliderMinimal" data-bs-slide-to="3" style="width: 8px; height: 8px; border-radius: 50%;"></button>
               </div>
               
               <button class="carousel-control-prev" type="button" data-bs-target="#courseSliderMinimal" data-bs-slide="prev" style="width: 30px; opacity: 0.7;">
                   <span style="color: white; font-size: 1.5rem; text-shadow: 0 2px 4px rgba(0,0,0,0.5);">←</span>
                   <span class="visually-hidden">Предыдущий</span>
               </button>
               <button class="carousel-control-next" type="button" data-bs-target="#courseSliderMinimal" data-bs-slide="next" style="width: 30px; opacity: 0.7;">
                   <span style="color: white; font-size: 1.5rem; text-shadow: 0 2px 4px rgba(0,0,0,0.5);">→</span>
                   <span class="visually-hidden">Следующий</span>
               </button>
           </div>
       </div>
   </div>

**Описание:** Четвертый вариант - минималистичный слайдер с простыми стрелками-символами (← и →) и маленькими круглыми индикаторами. Содержит полупрозрачные белые блоки с текстом, расположенные в левом нижнем углу. Высота контейнера - 400px. Используется для лаконичного представления информации.

Слайдер с контрастными стрелками-треугольниками и номером текущего слайда
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: html+django

   {# Слайдер с контрастными стрелками и счетчиком #}
   <div class="row justify-content-center">
       <div class="col-12 col-lg-10">
           <div id="courseSliderModern" class="carousel slide" data-bs-ride="carousel" data-bs-interval="5000">
               <div class="carousel-inner rounded-3 shadow-lg overflow-hidden" style="height: 450px;">
                   {# Слайд 1 - Программирование #}
                   <div class="carousel-item active h-100">
                       <img src="{% static 'images/slide1.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Курсы программирования">
                       <div class="carousel-caption d-none d-md-block" style="bottom: 60px; left: 50%; transform: translateX(-50%); background: rgba(0, 0, 0, 0.75); padding: 25px; border-radius: 12px; width: 90%; max-width: 600px; backdrop-filter: blur(5px);">
                           <h3 class="fw-bold text-white mb-3">Основы алгоритмизации и программирования</h3>
                           <p class="fs-5 text-light mb-0">Научитесь основам программирования и созданию алгоритмов с нуля</p>
                       </div>
                   </div>
                   
                   {# Слайд 2 - Веб-дизайн #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide2.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Веб-дизайн">
                       <div class="carousel-caption d-none d-md-block" style="bottom: 60px; left: 50%; transform: translateX(-50%); background: rgba(0, 0, 0, 0.75); padding: 25px; border-radius: 12px; width: 90%; max-width: 600px; backdrop-filter: blur(5px);">
                           <h3 class="fw-bold text-white mb-3">Основы веб-дизайна</h3>
                           <p class="fs-5 text-light mb-0">Освойте современные тенденции в создании веб-интерфейсов и UX/UI</p>
                       </div>
                   </div>
                   
                   {# Слайд 3 - Базы данных #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide3.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Базы данных">
                       <div class="carousel-caption d-none d-md-block" style="bottom: 60px; left: 50%; transform: translateX(-50%); background: rgba(0, 0, 0, 0.75); padding: 25px; border-radius: 12px; width: 90%; max-width: 600px; backdrop-filter: blur(5px);">
                           <h3 class="fw-bold text-white mb-3">Проектирование баз данных</h3>
                           <p class="fs-5 text-light mb-0">Изучите принципы проектирования и работы с современными базами данных</p>
                       </div>
                   </div>
                   
                   {# Слайд 4 - Документы #}
                   <div class="carousel-item h-100">
                       <img src="{% static 'images/slide4.jpg' %}" class="d-block w-100 h-100" style="object-fit: cover;" alt="Дипломы">
                       <div class="carousel-caption d-none d-md-block" style="bottom: 60px; left: 50%; transform: translateX(-50%); background: rgba(0, 0, 0, 0.75); padding: 25px; border-radius: 12px; width: 90%; max-width: 600px; backdrop-filter: blur(5px);">
                           <h3 class="fw-bold text-white mb-3">Официальные документы об образовании</h3>
                           <p class="fs-5 text-light mb-0">Получите сертификаты и дипломы после успешного завершения курсов</p>
                       </div>
                   </div>
               </div>
               
               {# Индикаторы с номером слайда #}
               <div class="carousel-indicators position-absolute" style="bottom: 20px; right: 20px; left: auto; margin: 0; flex-direction: row; gap: 8px;">
                   <div class="d-flex align-items-center bg-dark bg-opacity-75 rounded-pill px-3 py-2">
                       <span class="text-white fw-bold me-2" style="font-size: 0.9rem;">Слайд</span>
                       <button type="button" data-bs-target="#courseSliderModern" data-bs-slide-to="0" class="active mx-1" style="width: 12px; height: 12px; border-radius: 50%; border: 2px solid white; background-color: transparent;"></button>
                       <button type="button" data-bs-target="#courseSliderModern" data-bs-slide-to="1" class="mx-1" style="width: 12px; height: 12px; border-radius: 50%; border: 2px solid rgba(255,255,255,0.5); background-color: transparent;"></button>
                       <button type="button" data-bs-target="#courseSliderModern" data-bs-slide-to="2" class="mx-1" style="width: 12px; height: 12px; border-radius: 50%; border: 2px solid rgba(255,255,255,0.5); background-color: transparent;"></button>
                       <button type="button" data-bs-target="#courseSliderModern" data-bs-slide-to="3" class="mx-1" style="width: 12px; height: 12px; border-radius: 50%; border: 2px solid rgba(255,255,255,0.5); background-color: transparent;"></button>
                   </div>
               </div>
               
               {# Стрелки-треугольники #}
               <button class="carousel-control-prev" type="button" data-bs-target="#courseSliderModern" data-bs-slide="prev" style="width: 80px; opacity: 1; left: 20px;">
                   <div class="arrow-container-left d-flex align-items-center justify-content-center" style="width: 50px; height: 50px; background: rgba(255, 255, 255, 0.9); border-radius: 50%; box-shadow: 0 4px 12px rgba(0,0,0,0.2); transition: all 0.3s;">
                       <div style="width: 0; height: 0; border-top: 10px solid transparent; border-bottom: 10px solid transparent; border-right: 15px solid #333; margin-right: 3px;"></div>
                   </div>
                   <span class="visually-hidden">Предыдущий</span>
               </button>
               <button class="carousel-control-next" type="button" data-bs-target="#courseSliderModern" data-bs-slide="next" style="width: 80px; opacity: 1; right: 20px;">
                   <div class="arrow-container-right d-flex align-items-center justify-content-center" style="width: 50px; height: 50px; background: rgba(255, 255, 255, 0.9); border-radius: 50%; box-shadow: 0 4px 12px rgba(0,0,0,0.2); transition: all 0.3s;">
                       <div style="width: 0; height: 0; border-top: 10px solid transparent; border-bottom: 10px solid transparent; border-left: 15px solid #333; margin-left: 3px;"></div>
                   </div>
                   <span class="visually-hidden">Следующий</span>
               </button>
           </div>
       </div>
   </div>

   <style>
       .arrow-container-left:hover, .arrow-container-right:hover {
           background: rgba(255, 255, 255, 1) !important;
           transform: scale(1.1);
           box-shadow: 0 6px 16px rgba(0,0,0,0.3) !important;
       }
       
       .carousel-indicators button.active {
           background-color: white !important;
       }
       
       .carousel-indicators button:not(.active):hover {
           background-color: rgba(255,255,255,0.3) !important;
       }
   </style>

**Описание:** Пятый вариант - современный слайдер с контрастными стрелками-треугольниками в круглых кнопках и индикатором текущего слайда. Стрелки имеют эффекты наведения, а текстовые блоки содержат размытый фон (backdrop-filter). Высота контейнера - 450px. Используется для презентации ключевых преимуществ.

4 варианта карточки товара
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: html+django

   {# Наследование от базового шаблона #}
   {% extends 'base.html' %}

   {% block content %}
   <div class="container">
       <div class="row g-4">


           <!-- Card 1: Classic -->
           <div class="col-md-4">
               <div class="card shadow-sm">
                   <img src="https://picsum.photos/400/250?random=1" class="card-img-top" alt="image1">
                   <div class="card-body">
                       <h5 class="card-title">Классическая карточка</h5>
                       <p class="card-text">Простой и аккуратный вариант карточки в стиле Bootstrap.</p>
                       <a href="#" class="btn btn-primary">Подробнее</a>
                   </div>
               </div>
           </div>


           <!-- Card 2: Minimalistic -->
           <div class="col-md-4">
               <div class="card text-center border-dark shadow-sm">
                   <img src="https://picsum.photos/400/250?random=3" class="card-img-top" alt="image3">
                   <div class="card-body">
                       <h5 class="card-title">Минимализм</h5>
                       <p class="card-text">Строгий и лаконичный дизайн без лишних деталей.</p>
                       <button class="btn btn-dark">Читать</button>
                   </div>
               </div>
           </div>


           <!-- Card 3: With Badge -->
           <div class="col-md-4">
               <div class="card position-relative shadow-lg">
                   <span class="badge bg-danger position-absolute top-0 start-0 m-2 p-2 fs-6">New</span>
                   <img src="https://picsum.photos/400/250?random=4" class="card-img-top" alt="image4">
                   <div class="card-body">
                       <h5 class="card-title">Карточка с бейджем</h5>
                       <p class="card-text">Яркий бейдж привлекает внимание к важной информации.</p>
                       <a href="#" class="btn btn-danger">Смотреть</a>
                   </div>
               </div>
           </div>


           <!-- Card 4: Horizontal Card -->
           <div class="col-md-8">
               <div class="card flex-row shadow-sm">
                   <img src="https://picsum.photos/300/300?random=5" class="img-fluid" alt="image5" style="width:300px; object-fit:cover;">
                   <div class="card-body">
                       <h5 class="card-title">Горизонтальная карточка</h5>
                       <p class="card-text">Формат в виде горизонтальной ленты отлично подходит для списков.</p>
                       <a href="#" class="btn btn-success">Перейти</a>
                   </div>
               </div>
           </div>


       </div>
   </div>
   {% endblock %}

**Описание:** Четыре варианта карточек товара в стиле Bootstrap 5. Включают классическую вертикальную карточку, минималистичный вариант с темной рамкой, карточку с красным бейджом "New" и горизонтальную карточку для отображения в виде ленты. Все карточки используют сеточную систему Bootstrap для адаптивного расположения.

Кастомный админ-панель
^^^^^^^^^^^^^^^^^^^^^^^

Создание суперпользователя
--------------------------

Создайте суперпользователя в командной строке из директории проекта:

.. code-block:: bash

   python manage.py createsuperuser

Настройка URL-адресов (urls.py)
-------------------------------

В файле ``urls.py`` обновите маршруты:

.. code-block:: python
   :linenos:

   from django.urls import path
   from . import views
   
   urlpatterns = [
       # ... другие маршруты ...
       
       # Кастомная админка
       path('adminDash/', views.admin_page, name='admin'),
       path('adminDash/application/<int:application_id>/status/<str:status>/', 
            views.admin_update_application_status, 
            name='admin_update_status'),
       
       # Закомментируйте стандартную админку Django:
       # path('admin/', admin.site.urls),
   ]

Импорты в views.py
------------------

Добавьте необходимые импорты в начало файла ``views.py``:

.. code-block:: python
   :linenos:

   from django.contrib.admin.views.decorators import staff_member_required
   from .models import CustomUser
   from django.core.paginator import Paginator

Функции представления (views.py)
--------------------------------

Добавьте функции для работы с админ-панелью в конец ``views.py``:

.. code-block:: python
   :linenos:
   :emphasize-lines: 1,2,6,18,27

   @staff_member_required
   def admin_page(request):
       applications = Application.objects.all().order_by('-created_at')
       reviews = Review.objects.all().order_by('-created_at')
       users = CustomUser.objects.all()  
   
       # Фильтрация по статусу
       status_filter = request.GET.get('status')
       if status_filter in ['new', 'in_progress', 'completed']:
           applications = applications.filter(status=status_filter)
   
       # Пагинация
       paginator = Paginator(applications, 10)  # 10 заявок на страницу
       page_number = request.GET.get('page')
       page_obj = paginator.get_page(page_number)
   
       context = {
           'applications': page_obj,
           'reviews': reviews,
           'users': users,
           'status_filter': status_filter,
       }
       return render(request, 'admin-panel.html', context)
   
   
   @staff_member_required
   def admin_update_application_status(request, application_id, status):
       application = get_object_or_404(Application, id=application_id)
       if status in ['new', 'in_progress', 'completed']:
           application.status = status
           application.save()
           messages.success(request, f'Статус заявки {application.id} изменен на {application.get_status_display()}')
       return redirect('admin')

Шаблон админ-панели (admin-panel.html)
---------------------------------------

Создайте файл ``templates/admin-panel.html``:

.. code-block:: html+django
   :linenos:

   {% extends 'base.html' %}
   
   {% block title %}Админка - Корочки.есть{% endblock %}
   {% block content %}
   <h2>Административная панель</h2>
   
   <!-- Фильтр по статусу заявок -->
   <form method="get" class="mb-3 d-flex gap-2">
       <select name="status" class="form-select w-auto">
           <option value="">Все статусы</option>
           <option value="new" {% if status_filter == 'new' %}selected{% endif %}>Новая</option>
           <option value="in_progress" {% if status_filter == 'in_progress' %}selected{% endif %}>В процессе</option>
           <option value="completed" {% if status_filter == 'completed' %}selected{% endif %}>Завершено</option>
       </select>
       <button type="submit" class="btn btn-primary">Применить</button>
   </form>
   
   <!-- Таблица заявок -->
   <h3>Заявки</h3>
   <table class="table table-bordered table-hover">
       <thead>
           <tr>
               <th>ID</th>
               <th>Пользователь</th>
               <th>Курс</th>
               <th>Статус</th>
               <th>Действия</th>
           </tr>
       </thead>
       <tbody>
           {% for app in applications %}
           <tr>
               <td>{{ app.id }}</td>
               <td>{{ app.user.fio }}</td>
               <td>{{ app.course }}</td>
               <td>{{ app.get_status_display }}</td>
               <td>
                   <a href="{% url 'admin_update_status' app.id 'new' %}" class="btn btn-sm btn-success">Новый</a>
                   <a href="{% url 'admin_update_status' app.id 'in_progress' %}" class="btn btn-sm btn-warning">В процессе</a>
                   <a href="{% url 'admin_update_status' app.id 'completed' %}" class="btn btn-sm btn-secondary">Завершен</a>
               </td>
           </tr>
           {% empty %}
           <tr><td colspan="5" class="text-center">Заявок не найдено</td></tr>
           {% endfor %}
       </tbody>
   </table>
   
   <!-- Пагинация заявок -->
   <nav aria-label="Page navigation">
     <ul class="pagination">
       {% if applications.has_previous %}
       <li class="page-item">
         <a class="page-link" href="?{% if status_filter %}status={{ status_filter }}&{% endif %}page={{ applications.previous_page_number }}" aria-label="Previous">‹</a>
       </li>
       {% endif %}
       {% for num in applications.paginator.page_range %}
       <li class="page-item {% if applications.number == num %}active{% endif %}">
         <a class="page-link" href="?{% if status_filter %}status={{ status_filter }}&{% endif %}page={{ num }}">{{ num }}</a>
       </li>
       {% endfor %}
       {% if applications.has_next %}
       <li class="page-item">
         <a class="page-link" href="?{% if status_filter %}status={{ status_filter }}&{% endif %}page={{ applications.next_page_number }}" aria-label="Next">›</a>
       </li>
       {% endif %}
     </ul>
   </nav>
   
   <!-- Таблица пользователей -->
   <!-- <h3>Пользователи</h3>
   <table class="table table-striped">
       <thead>
           <tr>
               <th>ID</th>
               <th>ФИО</th>
               <th>Username</th>
               <th>Email</th>
           </tr>
       </thead>
       <tbody>
           {% for user in users %}
           <tr>
               <td>{{ user.id }}</td>
               <td>{{ user.fio }}</td>
               <td>{{ user.username }}</td>
               <td>{{ user.email }}</td>
           </tr>
           {% empty %}
           <tr><td colspan="4" class="text-center">Пользователей не найдено</td></tr>
           {% endfor %}
       </tbody>
   </table> -->
   
   <!-- Таблица отзывов -->
   <!-- <h3>Отзывы</h3>
   <table class="table table-hover">
       <thead>
           <tr>
               <th>ID</th>
               <th>Заявка</th>
               <th>Пользователь</th>
               <th>Оценка</th>
               <th>Текст</th>
           </tr>
       </thead>
       <tbody>
           {% for review in reviews %}
           <tr>
               <td>{{ review.id }}</td>
               <td>{{ review.application.id }}</td>
               <td>{{ review.application.user.fio }}</td>
               <td>{{ review.rating }}</td>
               <td>{{ review.text }}</td>
           </tr>
           {% empty %}
           <tr><td colspan="5" class="text-center">Отзывы не найдены</td></tr>
           {% endfor %}
       </tbody>
   </table> -->
   
   <!-- Всплывающие сообщения -->
   {% if messages %}
     {% for message in messages %}
       <div class="alert alert-{{ message.tags }} alert-dismissible fade show" role="alert">
         {{ message }}
         <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
       </div>
     {% endfor %}
   {% endif %}
   {% endblock %}

**Доступ:** Кастомная админка доступна по адресу ``/adminDash/`` только для пользователей с правами staff (``is_staff=True``). Для изменения статуса заявок используются кнопки с соответствующими статусами в таблице заявок.

Разметка Bootstrap
^^^^^^^^^^^^^^^^^^

В проекте используется Bootstrap 5 для создания адаптивного интерфейса. Ниже представлены основные шаблоны с применением сеточной системы и компонентов Bootstrap.

1. add_review.html - форма отзыва
---------------------------------

.. code-block:: html+django
   :linenos:

   {% extends 'base.html' %}

   {% block title %}Отзыв - Корочки.есть{% endblock %}
   {% block description %}Оставьте отзыв о пройденном курсе{% endblock %}
   {% block keywords %}отзыв, оценка, курс, обучение{% endblock %}

   {% block content %}
   <div class="container">
       <div class="row mb-4">
           <div class="col-12">
               <h2>Оставить отзыв</h2>
           </div>
       </div>

       <div class="row mb-4">
           <div class="col-12">
               <div class="card">
                   <div class="card-body">
                       <h5>Информация о курсе:</h5>
                       <p class="mb-1"><strong>Курс:</strong> {{ application.course }}</p>
                       <p class="mb-1"><strong>Дата начала:</strong> {{ application.desired_start_date|date:"d.m.Y" }}</p>
                       <p class="mb-0"><strong>Способ оплаты:</strong> {{ application.get_payment_method_display }}</p>
                   </div>
               </div>
           </div>
       </div>

       <form method="post" class="row g-3">
           {% csrf_token %}
           {% for field in form %}
           <div class="col-12">
               <label for="{{ field.id_for_label }}" class="form-label">{{ field.label }}</label>
               {{ field }}
               {% if field.errors %}
               <div class="text-danger small">
                   {% for error in field.errors %}
                   {{ error }}
                   {% endfor %}
               </div>
               {% endif %}
           </div>
           {% endfor %}

           <div class="col-12 d-flex gap-2">
               <button type="submit" class="btn btn-primary">Опубликовать отзыв</button>
               <a href="{% url 'applications' %}" class="btn btn-secondary">Отмена</a>
           </div>
       </form>
   </div>
   {% endblock %}

**Ключевые элементы Bootstrap:**
- Контейнер ``.container`` для центрирования контента
- Сетка ``.row`` + ``.col-12`` для размещения элементов
- Карточка ``.card`` + ``.card-body`` для блока информации о курсе
- Форма с классами ``.row g-3`` для вертикальных отступов
- Кнопки ``.btn`` с цветовыми классами ``.btn-primary``, ``.btn-secondary``
- Flex-утилита ``.d-flex gap-2`` для расположения кнопок

2. home.html - главная страница
-------------------------------

.. code-block:: html+django
   :linenos:

   {% extends 'base.html' %}
   {% load static %}

   {% block title %}Главная - Корочки.есть{% endblock %}
   {% block description %}Запишитесь на онлайн курсы программирования, веб-дизайна и баз данных. Официальные документы.{% endblock %}
   {% block keywords %}курсы, программирование, веб-дизайн, базы данных, обучение{% endblock %}

   {% block content %}
   <div class="container">
       <div class="row mb-5 text-center">
           <div class="col-12">
               <h1 class="display-4">Добро пожаловать на портал "Корочки.есть"</h1>
               <p class="lead">Онлайн курсы дополнительного профессионального образования</p>
               
               {% if not user.is_authenticated %}
               <div class="mt-4">
                   <a href="{% url 'register' %}" class="btn btn-primary btn-lg me-3">Начать обучение</a>
                   <a href="{% url 'login' %}" class="btn btn-outline-primary btn-lg">Войти в систему</a>
               </div>
               {% else %}
               <div class="mt-4">
                   <a href="{% url 'create_application' %}" class="btn btn-success btn-lg me-3">Подать заявку на курс</a>
                   <a href="{% url 'applications' %}" class="btn btn-outline-success btn-lg">Мои заявки</a>
               </div>
               {% endif %}
           </div>
       </div>

       <div class="row justify-content-center mb-5">
           <div class="col-12 col-lg-10 col-xl-8">
               <div id="courseSlider" class="carousel slide" data-bs-ride="carousel">
                   <div class="carousel-indicators">
                       {% for i in "0123" %}
                       <button type="button" data-bs-target="#courseSlider" data-bs-slide-to="{{ forloop.counter0 }}" class="{% if forloop.first %}active{% endif %}"></button>
                       {% endfor %}
                   </div>
                   <div class="carousel-inner rounded">
                       <div class="carousel-item active">
                           <img src="{% static 'images/slide1.jpg' %}" class="d-block w-100 slider-image" alt="Курсы программирования">
                           <div class="carousel-caption d-none d-md-block">
                               <h5>Основы алгоритмизации и программирования</h5>
                               <p>Научитесь основам программирования и созданию алгоритмов</p>
                           </div>
                       </div>
                       <div class="carousel-item">
                           <img src="{% static 'images/slide2.jpg' %}" class="d-block w-100 slider-image" alt="Веб-дизайн">
                           <div class="carousel-caption d-none d-md-block">
                               <h5>Основы веб-дизайна</h5>
                               <p>Освойте современные тенденции в создании веб-интерфейсов</p>
                           </div>
                       </div>
                       <div class="carousel-item">
                           <img src="{% static 'images/slide3.jpg' %}" class="d-block w-100 slider-image" alt="Базы данных">
                           <div class="carousel-caption d-none d-md-block">
                               <h5>Основы проектирования баз данных</h5>
                               <p>Изучите принципы проектирования и работы с базами данных</p>
                           </div>
                       </div>
                       <div class="carousel-item">
                           <img src="{% static 'images/slide4.jpg' %}" class="d-block w-100 slider-image" alt="Дипломы">
                           <div class="carousel-caption d-none d-md-block">
                               <h5>Получите документы об образовании</h5>
                               <p>Официальные документы после успешного завершения курсов</p>
                           </div>
                       </div>
                   </div>
                   <button class="carousel-control-prev" type="button" data-bs-target="#courseSlider" data-bs-slide="prev">
                       <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                       <span class="visually-hidden">Предыдущий</span>
                   </button>
                   <button class="carousel-control-next" type="button" data-bs-target="#courseSlider" data-bs-slide="next">
                       <span class="carousel-control-next-icon" aria-hidden="true"></span>
                       <span class="visually-hidden">Следующий</span>
                   </button>
               </div>
           </div>
       </div>

       <div class="row">
           <div class="col-md-4 mb-4">
               <div class="card h-100 text-center">
                   <div class="card-body">
                       <h5 class="card-title">🎯 Основы алгоритмизации</h5>
                       <p class="card-text">Изучите основы программирования, алгоритмы и структуры данных. Подходит для начинающих.</p>
                   </div>
               </div>
           </div>
           <div class="col-md-4 mb-4">
               <div class="card h-100 text-center">
                   <div class="card-body">
                       <h5 class="card-title">🎨 Веб-дизайн</h5>
                       <p class="card-text">Освойте создание современных веб-интерфейсов, UX/UI дизайн и работу с графикой.</p>
                   </div>
               </div>
           </div>
           <div class="col-md-4 mb-4">
               <div class="card h-100 text-center">
                   <div class="card-body">
                       <h5 class="card-title">🗄️ Базы данных</h5>
                       <p class="card-text">Научитесь проектировать и работать с базами данных, писать SQL запросы.</p>
                   </div>
               </div>
           </div>
       </div>
   </div>
   {% endblock %}

   {% block scripts %}
   <script>
   document.addEventListener('DOMContentLoaded', function() {
       var myCarousel = document.getElementById('courseSlider');
       var carousel = new bootstrap.Carousel(myCarousel, {
           interval: 3000,
           wrap: true
       });
   });
   </script>
   {% endblock %}

**Ключевые элементы Bootstrap:**
- Типографика: ``.display-4``, ``.lead`` для заголовков
- Кнопки разных размеров: ``.btn-lg``
- Карусель (слайдер) ``.carousel`` с индикаторами ``.carousel-indicators`` и навигацией
- Адаптивная сетка: ``.col-md-4`` для карточек курсов (3 колонки на десктопе, 1 на мобильных)
- Карточки ``.card`` с ``.h-100`` для одинаковой высоты
- Отзывчивые классы: ``col-12 col-lg-10 col-xl-8`` для ограничения ширины слайдера

3. application.html - страница заявок
-------------------------------------

.. code-block:: html+django
   :linenos:

   {% extends 'base.html' %}
   {% load static %}

   {% block title %}Мои заявки - Корочки.есть{% endblock %}
   {% block description %}Просмотр ваших заявок на обучение и отзывов{% endblock %}
   {% block keywords %}заявки, обучение, отзывы, статусы{% endblock %}

   {% block content %}
   <div class="container">
       <div class="row mb-4 align-items-center">
           <div class="col-md-6">
               <h2>Мои заявки</h2>
           </div>
           <div class="col-md-6 text-md-end">
               <a href="{% url 'create_application' %}" class="btn btn-primary">➕ Новая заявка</a>
           </div>
       </div>

       {% if applications %}
       <div class="row">
           {% for application in applications %}
           <div class="col-md-6 mb-4">
               <div class="card h-100 application-card
                   {% if application.status == 'new' %}application-new
                   {% elif application.status == 'in_progress' %}application-in-progress
                   {% elif application.status == 'completed' %}application-completed{% endif %}">
                   <div class="card-body">
                       <div class="d-flex justify-content-between align-items-start mb-2">
                           <h5 class="card-title">{{ application.get_course_display }}</h5>
                           <span class="badge 
                               {% if application.status == 'new' %}bg-success
                               {% elif application.status == 'in_progress' %}bg-warning
                               {% else %}bg-secondary{% endif %}">
                               {{ application.get_status_display }}
                           </span>
                       </div>
                       <p class="card-text mb-2">
                           <strong>Дата начала:</strong> {{ application.desired_start_date|date:"d.m.Y" }}<br>
                           <strong>Способ оплаты:</strong> {{ application.get_payment_method_display }}<br>
                           <strong>Подана:</strong> {{ application.created_at|date:"d.m.Y H:i" }}
                       </p>

                       {% if application.status == 'completed' %}
                           <div class="mt-3">
                               {% if application.review %}
                                   <div class="alert alert-info">
                                       <strong>Ваш отзыв:</strong><br>
                                       Оценка: {{ application.review.rating }}/5<br>
                                       {{ application.review.text }}
                                   </div>
                               {% else %}
                                   <a href="{% url 'add_review' application.id %}" class="btn btn-outline-primary btn-sm">📝 Оставить отзыв</a>
                               {% endif %}
                           </div>
                       {% endif %}
                   </div>
               </div>
           </div>
           {% endfor %}
       </div>
       {% else %}
       <div class="row py-5">
           <div class="col-12 text-center">
               <h4>У вас пока нет заявок</h4>
               <p class="text-muted">Подайте первую заявку на обучение!</p>
               <a href="{% url 'create_application' %}" class="btn btn-primary">Подать заявку</a>
           </div>
       </div>
       {% endif %}
   </div>
   {% endblock %}

**Ключевые элементы Bootstrap:**
- Выравнивание с помощью ``.align-items-center`` и ``.text-md-end``
- Бейджи ``.badge`` с цветами в зависимости от статуса
- Flex-утилиты: ``.d-flex justify-content-between align-items-start``
- Адаптивная сетка ``.col-md-6`` (2 колонки на десктопе)
- Уведомления ``.alert alert-info`` для отображения отзывов
- Кнопка-ссылка ``.btn-outline-primary`` для оставления отзыва

4. admin-panel.html - админ-панель
----------------------------------

.. code-block:: html+django
   :linenos:

   {% extends 'base.html' %}

   {% block title %}Админка - Корочки.есть{% endblock %}
   {% block content %}
   <div class="container">
       <div class="row mb-4">
           <div class="col-12">
               <h2>Административная панель</h2>
           </div>
       </div>

       <!-- Фильтр по статусу заявок -->
       <div class="row mb-3">
           <div class="col-12">
               <form method="get" class="d-flex gap-2">
                   <select name="status" class="form-select w-auto">
                       <option value="">Все статусы</option>
                       <option value="new" {% if status_filter == 'new' %}selected{% endif %}>Новая</option>
                       <option value="in_progress" {% if status_filter == 'in_progress' %}selected{% endif %}>В процессе</option>
                       <option value="completed" {% if status_filter == 'completed' %}selected{% endif %}>Завершено</option>
                   </select>
                   <button type="submit" class="btn btn-primary">Применить</button>
               </form>
           </div>
       </div>

       <!-- Таблица заявок -->
       <div class="row mb-4">
           <div class="col-12">
               <h3>Заявки</h3>
               <table class="table table-bordered table-hover">
                   <thead>
                       <tr>
                           <th>ID</th>
                           <th>Пользователь</th>
                           <th>Курс</th>
                           <th>Статус</th>
                           <th>Действия</th>
                       </tr>
                   </thead>
                   <tbody>
                       {% for app in applications %}
                       <tr>
                           <td>{{ app.id }}</td>
                           <td>{{ app.user.fio }}</td>
                           <td>{{ app.course }}</td>
                           <td>{{ app.get_status_display }}</td>
                           <td>
                               <a href="{% url 'admin_update_status' app.id 'new' %}" class="btn btn-sm btn-success">Новый</a>
                               <a href="{% url 'admin_update_status' app.id 'in_progress' %}" class="btn btn-sm btn-warning">В процессе</a>
                               <a href="{% url 'admin_update_status' app.id 'completed' %}" class="btn btn-sm btn-secondary">Завершен</a>
                           </td>
                       </tr>
                       {% empty %}
                       <tr><td colspan="5" class="text-center">Заявок не найдено</td></tr>
                       {% endfor %}
                   </tbody>
               </table>
           </div>
       </div>

       <!-- Пагинация -->
       <div class="row mb-4">
           <div class="col-12 d-flex justify-content-center">
               <nav aria-label="Page navigation">
                   <ul class="pagination">
                       {% if applications.has_previous %}
                       <li class="page-item">
                           <a class="page-link" href="?{% if status_filter %}status={{ status_filter }}&{% endif %}page={{ applications.previous_page_number }}" aria-label="Previous">‹</a>
                       </li>
                       {% endif %}
                       {% for num in applications.paginator.page_range %}
                       <li class="page-item {% if applications.number == num %}active{% endif %}">
                           <a class="page-link" href="?{% if status_filter %}status={{ status_filter }}&{% endif %}page={{ num }}">{{ num }}</a>
                       </li>
                       {% endfor %}
                       {% if applications.has_next %}
                       <li class="page-item">
                           <a class="page-link" href="?{% if status_filter %}status={{ status_filter }}&{% endif %}page={{ applications.next_page_number }}" aria-label="Next">›</a>
                       </li>
                       {% endif %}
                   </ul>
               </nav>
           </div>
       </div>

       <!-- Таблица пользователей -->
   <!-- <h3>Пользователи</h3>
   <table class="table table-striped">
       <thead>
           <tr>
               <th>ID</th>
               <th>ФИО</th>
               <th>Username</th>
               <th>Email</th>
           </tr>
       </thead>
       <tbody>
           {% for user in users %}
           <tr>
               <td>{{ user.id }}</td>
               <td>{{ user.fio }}</td>
               <td>{{ user.username }}</td>
               <td>{{ user.email }}</td>
           </tr>
           {% empty %}
           <tr><td colspan="4" class="text-center">Пользователей не найдено</td></tr>
           {% endfor %}
       </tbody>
   </table> -->

   <!-- Таблица отзывов -->
   <!-- <h3>Отзывы</h3>
   <table class="table table-hover">
       <thead>
           <tr>
               <th>ID</th>
               <th>Заявка</th>
               <th>Пользователь</th>
               <th>Оценка</th>
               <th>Текст</th>
           </tr>
   </thead>
       <tbody>
           {% for review in reviews %}
           <tr>
               <td>{{ review.id }}</td>
               <td>{{ review.application.id }}</td>
               <td>{{ review.application.user.fio }}</td>
               <td>{{ review.rating }}</td>
               <td>{{ review.text }}</td>
           </tr>
           {% empty %}
           <tr><td colspan="5" class="text-center">Отзывы не найдены</td></tr>
           {% endfor %}
       </tbody>
   </table> -->

       <!-- Всплывающие сообщения -->
       {% if messages %}
           <div class="row">
               <div class="col-12">
                   {% for message in messages %}
                       <div class="alert alert-{{ message.tags }} alert-dismissible fade show" role="alert">
                           {{ message }}
                           <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
                       </div>
                   {% endfor %}
               </div>
           </div>
       {% endif %}
   </div>
   {% endblock %}

**Ключевые элементы Bootstrap:**
- Таблицы ``.table table-bordered table-hover`` с сортировкой строк
- Кнопки управления ``.btn-sm`` для компактных действий
- Пагинация ``.pagination`` с активными элементами
- Select-элемент ``.form-select w-auto`` для фильтрации
- Всплывающие уведомления ``.alert`` с разными типами ``alert-{{ message.tags }}``
- Flex-утилиты для центрирования пагинации ``.d-flex justify-content-center``

**Общие принципы использования Bootstrap в проекте:**
1. Все шаблоны наследуют от ``base.html``
2. Используется сеточная система для адаптивного дизайна
3. Компоненты Bootstrap (карточки, таблицы, формы) стилизуются стандартными классами
4. Адаптивность достигается через классы ``col-md-*``, ``col-lg-*``, ``col-xl-*``
5. Для выравнивания и расположения элементов используются flex-утилиты
6. Все формы используют стили Bootstrap ``.form-control``, ``.form-label``

Добавление установленных (кастомных) шрифтов
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Для добавления кастомных шрифтов в проект необходимо выполнить следующие шаги:

1. Создание структуры папок
--------------------------------

В папке ``static`` создайте папку ``fonts`` и поместите туда файлы шрифтов в форматах TTF, WOFF или WOFF2:

.. code-block:: bash

   korochki/
   ├── static/
   │   ├── css/
   │   │   └── styles.css
   │   ├── images/
   │   └── fonts/                    # ← Создайте эту папку
   │       ├── OpenSans-Regular.ttf  # Пример файлов шрифтов
   │       ├── OpenSans-SemiBold.ttf
   │       └── OpenSans-Bold.ttf
   └── ...

2. Добавление шрифтов в styles.css
-----------------------------------

В файле ``static/css/styles.css`` после блока цветовой палитры добавьте декларации шрифтов:

.. code-block:: css
   :linenos:
   :emphasize-lines: 1-18

   /* ===== КАСТОМНЫЕ ШРИФТЫ ===== */
   @font-face {
       font-family: 'Open Sans';
       src: url('../fonts/OpenSans-Regular.ttf') format('truetype');
       font-weight: 400;
       font-style: normal;
       font-display: swap;
   }
   
   @font-face {
       font-family: 'Open Sans';
       src: url('../fonts/OpenSans-SemiBold.ttf') format('truetype');
       font-weight: 600;
       font-style: normal;
       font-display: swap;
   }
   
   @font-face {
       font-family: 'Open Sans';
       src: url('../fonts/OpenSans-Bold.ttf') format('truetype');
       font-weight: 700;
       font-style: normal;
       font-display: swap;
   }
   
   /* ===== ОБЩИЕ СТИЛИ ===== */
   body {
       background-color: var(--light-gray) !important;
       color: var(--text-dark) !important;
       font-family: 'Open Sans', 'SF Pro Display', system-ui, -apple-system, sans-serif !important;
   }

3. Примеры различных вариантов подключения шрифтов
---------------------------------------------------

**Вариант 1: Один шрифт с несколькими начертаниями**

.. code-block:: css

   @font-face {
       font-family: 'Montserrat';
       src: url('../fonts/Montserrat-Regular.woff2') format('woff2');
       font-weight: 400;
       font-style: normal;
       font-display: swap;
   }
   
   @font-face {
       font-family: 'Montserrat';
       src: url('../fonts/Montserrat-Italic.woff2') format('woff2');
       font-weight: 400;
       font-style: italic;
       font-display: swap;
   }
   
   @font-face {
       font-family: 'Montserrat';
       src: url('../fonts/Montserrat-Bold.woff2') format('woff2');
       font-weight: 700;
       font-style: normal;
       font-display: swap;
   }
   
   body {
       font-family: 'Montserrat', sans-serif;
   }

**Вариант 2: Несколько разных шрифтов**

.. code-block:: css

   @font-face {
       font-family: 'Roboto Slab';
       src: url('../fonts/RobotoSlab-Regular.ttf') format('truetype');
       font-weight: 400;
       font-display: swap;
   }
   
   @font-face {
       font-family: 'Roboto Mono';
       src: url('../fonts/RobotoMono-Regular.ttf') format('truetype');
       font-weight: 400;
       font-display: swap;
   }
   
   /* Основной текст */
   body {
       font-family: 'Roboto Slab', serif;
   }
   
   /* Для кода */
   code, pre {
       font-family: 'Roboto Mono', monospace;
   }

**Вариант 3: Шрифт с поддержкой кириллицы**

.. code-block:: css

   @font-face {
       font-family: 'PT Sans';
       src: url('../fonts/PTSans-Regular.ttf') format('truetype');
       font-weight: 400;
       font-display: swap;
       unicode-range: U+0400-04FF; /* Кириллический диапазон */
   }

4. Настройка специфичных элементов
-----------------------------------

После подключения шрифтов можно настроить их применение для различных элементов:

.. code-block:: css

   /* Для заголовков */
   h1, h2, h3, h4, h5, h6 {
       font-family: 'Open Sans', sans-serif;
       font-weight: 700; /* Использует Bold начертание */
   }
   
   /* Для кнопок */
   .btn {
       font-family: 'Open Sans', sans-serif;
       font-weight: 600; /* Использует SemiBold начертание */
   }
   
   /* Для навигации */
   .navbar-brand, .nav-link {
       font-family: 'Open Sans', sans-serif;
       font-weight: 500;
   }
   
   /* Для карточек */
   .card-title {
       font-family: 'Open Sans', sans-serif;
       font-weight: 600;
   }
   
   .card-text {
       font-family: 'Open Sans', sans-serif;
       font-weight: 400;
       line-height: 1.6;
   }

5. Поддержка различных форматов шрифтов
----------------------------------------

Для лучшей совместимости с разными браузерами рекомендуется использовать несколько форматов:

.. code-block:: css

   @font-face {
       font-family: 'CustomFont';
       src: url('../fonts/CustomFont.woff2') format('woff2'),
            url('../fonts/CustomFont.woff') format('woff'),
            url('../fonts/CustomFont.ttf') format('truetype');
       font-weight: 400;
       font-style: normal;
       font-display: swap;
   }

**Пояснения к параметрам:**
- ``font-family``: имя шрифта, которое будет использоваться в CSS
- ``src``: путь к файлу шрифта и его формат
- ``font-weight``: толщина шрифта (400 - normal, 600 - semibold, 700 - bold)
- ``font-style``: стиль (normal, italic)
- ``font-display: swap``: гарантирует, что текст будет виден сразу, даже если шрифт еще не загрузился
- ``unicode-range``: ограничение набора символов (полезно для кириллических шрифтов)

6. Практический пример использования
-------------------------------------

Для проекта "Корочки.есть" с шрифтом "Open Sans":

.. code-block:: css

   /* ===== КАСТОМНЫЕ ШРИФТЫ ===== */
   @font-face {
       font-family: 'Open Sans';
       src: url('../fonts/OpenSans-Light.ttf') format('truetype');
       font-weight: 300;
       font-style: normal;
       font-display: swap;
   }
   
   @font-face {
       font-family: 'Open Sans';
       src: url('../fonts/OpenSans-Regular.ttf') format('truetype');
       font-weight: 400;
       font-style: normal;
       font-display: swap;
   }
   
   @font-face {
       font-family: 'Open Sans';
       src: url('../fonts/OpenSans-SemiBold.ttf') format('truetype');
       font-weight: 600;
       font-style: normal;
       font-display: swap;
   }
   
   @font-face {
       font-family: 'Open Sans';
       src: url('../fonts/OpenSans-Bold.ttf') format('truetype');
       font-weight: 700;
       font-style: normal;
       font-display: swap;
   }
   
   /* ===== ОБЩИЕ СТИЛИ ===== */
   body {
       background-color: var(--light-gray) !important;
       color: var(--text-dark) !important;
       font-family: 'Open Sans', system-ui, -apple-system, sans-serif !important;
       font-weight: 400;
   }
   
   /* Специфичные настройки */
   .display-4, .display-5, .display-6 {
       font-family: 'Open Sans', sans-serif !important;
       font-weight: 700 !important;
   }
   
   .navbar-brand {
       font-family: 'Open Sans', sans-serif !important;
       font-weight: 600 !important;
   }
   
   .btn {
       font-family: 'Open Sans', sans-serif !important;
       font-weight: 600 !important;
   }

**Важные замечания:**
1. Убедитесь, что пути к файлам шрифтов указаны правильно относительно файла ``styles.css``
2. Формат файла должен соответствовать указанному в ``format()``
3. Используйте ``font-display: swap`` для улучшения производительности
4. Проверьте поддержку шрифтом кириллических символов, если проект на русском языке
5. Для файлов TTF используйте ``format('truetype')``, а не ``format('ttf')``

ER-диаграмма
^^^^^^^^^^^^

.. image:: /_static/images/Er-demo.png
   :width: 800
   :height: 600
   :scale: 100%
   :alt: Entity-Relationship диаграмма
   :align: center
   
**Сущности базы данных:**
   
1. **CustomUser** - модель пользователя с полями:
   - id, username, email, fio (ФИО)
   - is_staff, is_active, date_joined
   
2. **Application** - заявка на курс:
   - id, user (ForeignKey), course, status
   - desired_start_date, payment_method
   - created_at, updated_at
   
3. **Review** - отзыв о курсе:
   - id, application (OneToOne), rating, text
   - created_atг