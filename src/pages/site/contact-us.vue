<template>
  <div>
    <BlockMap />

    <PageHeader
      title="Связаться с нами"
      :breadcrumb="[
        { title: 'Главная', url: '' },
        { title: 'Связаться с нами', url: '' },
      ]"
    />

    <div class="block">
      <div class="container">
        <div class="card mb-0">
          <div class="card-body contact-us">
            <div class="contact-us__container">
              <div class="row">
                <div class="col-12 col-lg-6 pb-4 pb-lg-0">
                  <h4 class="contact-us__header card-title">Наш адрес</h4>

                  <div class="contact-us__address">
                    <p>
                      715 Fake Ave, Apt. 34, New York, NY 10021 USA
                      <br />
                      Email: stroyka@example.com
                      <br />
                      Телефон номер 87029371515
                    </p>

                    <p>
                      <strong>Часы работы</strong>
                      <br />
                      Monday to Friday: 8am-8pm
                      <br />
                      Saturday: 8am-6pm
                      <br />
                      Sunday: 10am-4pm
                    </p>

                    <p>
                      <strong>Comment</strong>
                      <br />
                      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                      Curabitur suscipit suscipit mi, non tempor nulla finibus
                      eget. Lorem ipsum dolor sit amet, consectetur adipiscing
                      elit.
                    </p>
                  </div>
                </div>

                <div class="col-12 col-lg-6">
                  <h4 class="contact-us__header card-title">
                    Оставьте нам сообщение
                  </h4>

                  <form>
                    <div class="form-row">
                      <div class="form-group col-md-6">
                        <label for="form-name">Имя</label>
                        <input
                          id="form-name"
                          class="form-control"
                          type="text"
                          placeholder="Имя"
                        />
                      </div>
                      <div class="form-group col-md-6">
                        <label for="form-email">Емайл</label>
                        <input
                          id="form-email"
                          class="form-control"
                          type="email"
                          placeholder="Емайл Адрес"
                        />
                      </div>
                    </div>
                    <div class="form-group">
                      <label for="form-subject">Предмет</label>
                      <input
                        id="form-subject"
                        class="form-control"
                        type="text"
                        placeholder="Предмет"
                      />
                    </div>
                    <div class="form-group">
                      <label for="form-message">Сообщение</label>
                      <textarea
                        id="form-message"
                        class="form-control"
                        :rows="4"
                      />
                    </div>
                    <button type="submit" class="btn btn-primary">
                     Отправить сообщение
                    </button>
                  </form>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import PageHeader from "~/components/shared/page-header.vue";
import BlockMap from "~/components/blocks/block-map.vue";

@Component({
  components: { PageHeader, BlockMap },
  head() {
    return {
      title: "Contact Us",
    };
  },
})
export default class SitePageContactUs extends Vue {}
</script>
