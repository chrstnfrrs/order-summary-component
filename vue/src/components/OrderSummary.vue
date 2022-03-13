<template>
  <main class="order-summary__card">
    <figure>
      <img
        class="order-summary__illustration"
        src="../assets/illustration-hero.svg"
        alt=""
      />
    </figure>
    <div class="order-summary__body">
      <h1 class="order-summary__heading">Order Summary</h1>
      <p class="order-summary__text">
        You can now listen to millions of songs, audiobooks, and podcasts on any
        device anywhere you like!
      </p>
      <OrderItem />
      <button
        class="order-summary__btn order-summary__btn--primary"
        type="button"
      >
        Proceed to Payment
      </button>
      <button
        class="order-summary__btn order-summary__btn--secondary"
        type="button"
      >
        Cancel Order
      </button>
    </div>
  </main>
</template>

<script>
import OrderItem from "./OrderItem.vue";

export default {
  name: "OrderSummary",
  components: {
    OrderItem,
  },
};
</script>

<style lang="scss">
.order-summary {
  &__illustration {
    border-radius: 1.25rem 1.25rem 0 0;
  }
  &__card {
    background-color: var(--white);
    border-radius: 1.25rem;
    max-width: 28.125rem;
    filter: drop-shadow(0 40px 40px hsl(228, 87%, 39%, 15.18%));
  }
  &__body {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2rem 3rem 1rem;
    @media only screen and (max-width: 660px) {
      padding: 2rem 1.5rem 1rem;
    }
  }
  &__heading {
    color: var(--dark-blue);
    font-size: 1.75rem;
    font-weight: 900;
    margin: 1rem;
  }
  &__text {
    color: var(--desaturated-blue);
    font-weight: 500;
    text-align: center;
    margin-bottom: 1rem;
    @media only screen and (max-width: 660px) {
      padding: 0 0.25rem;
    }
  }
  &__btn {
    display: flex;
    width: 100%;
    justify-content: center;
    font-size: 0.9375rem;
    font-weight: 900;
    border: none;
    outline: none;
    padding: 1rem 0;
    border-radius: 0.6875rem;
    margin-bottom: 0.5rem;
    cursor: pointer;
    &--primary {
      background: var(--bright-blue);
      color: var(--white);
      filter: drop-shadow(0 20px 20px hsl(245, 75%, 52%, 19.03%));
    }
    &--secondary {
      background: var(--white);
      color: var(--desaturated-blue);
    }
  }
}
</style>
